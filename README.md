# Features

Features are the technicals building blocks of Inmemori revenue model. It's through them that we monetize the service. we can think of them as revenue streams.

Every time a feature is used, a new `Order` object is created. 
An `order` object contains the relevant informations associated with that interaction.

Each feature is assigned a unique key, and possible settings.

## Active Features

```
[
    { 
        key: 'donation'
      , emails: 'client,admin'
    }
  , { 
        key: 'flower' 
      , emails: 'client,team'
    }
  , { 
        key: 'book' 
      , emails: 'client,team'
    }
  , { 
        key: 'gcard'
      , emails: 'client,team'
    }
]
```

## Emails & templates

For example, if you set `emails: 'client,team'` for the feature key `flower`, then 2 emails will be sent with the following template names `client-flower` & `team-flower`.  
Make sure those templates exists in Sendgrid, for each language, otherwise an error will be thrown.

Each Sendgrid template has access to an `order` object, giving context to the content of your mail.
You can access the information by accessing the `ctx` key followed by your desired path
```
Bonjour {{ctx.client.name}} ! votre reçu est le n°{{ctx.tx.ch_id}}
```


## Order Definition

```
{
  "_id": "BJB-HTmHXGS",
  "cat": "2019-07-22T14:10:05.173Z",
  "cat_f": "22/07/2019 - 16:10 (Paris)",
  "shipping": {
    "name": "Eglise Saint Sébastien",
    "address": "Place Dr Joseph Chevillon, 13190 Allauch, France",
    "date": "2019-08-15T08:00:00.000Z",
    "date_f": "15/08/2019 - 10:00",
    "amount": 890,
    "amount_f": "8.90€"
  },
  "invoice": {
    "name": "Bruno Hervé",
    "address": "25, boulevard Aristide Briand",
    "city": "Le Cannet",
    "zipcode": "06110",
    "vat": "",
    "phone": "0698736050",
    "email": "bruno.h@gmail.com"
  },
  "item": {
    "name": "Souvenir",
    "product": "6P04",
    "qty": 1,
    "amount": 500,
    "amount_total_f": "5.00€",
    "amount_f": "5.00€"
  },
  "tx": {
    "amount": 1390,
    "amount_f": "13.90€"
    "currency": "eur",
    "pi_id": "pi_1Ez2CyDvcFOuP8N2XYHxCD7v",
    "pm_id": "pm_1Ez2CxDvcFOuP8N24EejJg4f",
    "ch_id": "ch_1Ez2DHDvcFOuP8N2jJiZVBrn",
    "ca_id": "acct_1EuxorG8voAk1bsZ"
  },
  "meta": {
    "message": "un joli message ❤"
  }
}
```


# Settings

Features settings can applied at different levels, each level overriding it's parent level settings.  
The level of granularity comes in the following order :

- [zones.md](https://github.com/imstack/config/blob/main/zone.md)
- [partners.json](https://github.com/imstack/config/blob/main/partners.json)
- [agencies.json](https://github.com/imstack/config/blob/main/agencies.json)
- [slugs.json](https://github.com/imstack/config/blob/main/slugs.json)

ex: partners.json
```
"interflora-fr": {
  "features": {
     "flower": { "catalog": "interflora-fr", "hours": -2, "caid":"acct_1DJiYIGMg492Tw0T", cut: 20 }
  }
}

"scf-marseille": {
  "features": {
      "flower": "interflora-fr"
    , "book": false
  }
}
```

After you've made modification to the settings, wait for github cache to clear (circa 5m), then synchronize the new data on our API in order to take effect. just click this link to sync : https://api.inmemori.com/utils/sync
