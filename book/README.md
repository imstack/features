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
        "fr":"Le livre InMemori rassemble l’ensemble des messages et photos partagés par vos proches. Sa mise en page est réalisée par les équipes d'InMemori. \n\nVotre livre est imprimé et façonné par Escourbiac, artisan imprimeur à Graulhet, au cœur du Tarn. \nIl a été primé par 3 Cadrats d’Or, le plus ancien et le plus prestigieux des concours de l’imprimerie française qui récompense la qualité d’impression. \n\nCaractéristiques techniques : \n* impression quadri - format : 150 x 210 mm\n* marquage à chaud du titre « Hommages » et embossage cuvette pour la photo \n* rainage, pliage et collage des soufflets (accordéon) à la main. \n* papier couverture : Wibalin coloris bleu\n* papier intérieur : Symbol Tatami Ivoire 150 g/m2.",
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
