# Book Feature

### Book Offer Exemple

```
{
  "shipping":{
    "price":8.90,
    "info":"Livraison France uniquement"
  },
  "prices": [
      [0,4,   20]
    , [4,8,   25]
    , [8,12,  35]
    , [12,16, 40]
    , [16,20, 45]
    , [20,24, 50]
    , [24,28, 55]
    , [28,32, 60]
    , [32,36, 65]
    , [36,40, 70]
    , [40,44, 75]
    , [44,48, 80]
    , [48,52, 90]
    , [52,56, 95]
    , [56,60, 100]
    , [60,64, 100]
  ],
  "catalog":[
    {
      "product":"B1",
      "name":{
        "fr":"Livre InMemori",
        "en":"My InMemori book ",
        "es":"Mi libro InMemori"
      },
      "desc":{
        "fr":"Le livre InMemori rassemble l’ensemble des messages et photos partagés par vos proches. Sa mise en page est réalisée par les équipes d'InMemori. \n\nCaractéristiques techniques : \n* Format accordéon : 150 x 210 mm \n* Papier de qualité : 150 g / m2\n* Imprimé et façonné en France\n* Livraison en Europe uniquement",
        "en":"Accordion-style\nHigh-quality ivory-colored paper\nTitle in a bronze shade\nCover photo identical to the InMemori page’s main photo\nMade by an artisanal printer\n\nThe InMemori book is a beautiful keepsake of all the messages and photos shared by close ones.\nThe layout is formatted by InMemori team, so you don’t have to spend hours doing it yourself.",
        "es":"Pliegue de acordeón\nPapel de color marfil de alta calidad\nTítulo en color bronce\nFoto de portada idéntica a la foto principal elegida para la página\nDiseñado por un artesano\n\nEl libro InMemori es un hermoso objeto para conservar las bellas palabras y fotos escritas.\nSu diseño es realizado por los equipos de InMemori, lo que evita largas horas de trabajo."
      },
      "imgs":[
        "https://res.cloudinary.com/inmemori/image/upload/fl_lossy,f_auto/InMemori-book-3_ulc04r",
        "https://res.cloudinary.com/inmemori/image/upload/fl_lossy,f_auto/InMemori-book-2_rn9m8j",
        "https://res.cloudinary.com/inmemori/image/upload/fl_lossy,f_auto/InMemori-book-1_yrqc9k",
        "https://res.cloudinary.com/inmemori/image/upload/fl_lossy,f_auto/InMemori-book-4_awbkvl"
      ]
    }
  ]
}
```

### Model/API user.book

```
"book": {
    "range": "8-12",
    "price_f": "47.00€",
    "price": 4700,
    "nbPages": 11,
    "nbImgs": 15,
    "nbChars": 9351
}
```

### Average data

```
{
    charsByLine: 65
  , linesByPage: 30
  , charsByTitle: 30
  , titlesByPage: 4
  , imgsByPage: 3
}
```
