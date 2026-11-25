# Icone

Icone pubbliche per le applicazioni di Francisco (Google Apps Script e HTML).
Il repo è pubblico apposta: Apps Script accetta come favicon solo l'URL pubblico di un'immagine.

## Struttura
Una cartella per app.

### consumi/ (App Consumi)
- `consumi-icon.svg`: icona completa (C a quattro colori: corrente, gas, acqua, spazzatura, su fondo blu scuro)
- `consumi-mark.svg`: solo il simbolo, senza fondo
- `consumi-icon-32.png`, `-64.png`, `-192.png`, `-512.png`: PNG ricavati dall'SVG
- `favicon.ico`: 16, 32, 48 e 64 px
- `consumi-favicon-32.png`, `consumi-favicon-64.png`: solo la C, senza fondo e con poco margine, per la scheda del browser (sta in riga con le icone delle altre schede)

Uso in Apps Script (`Code.gs`):

```js
const ICONA_URL = 'https://raw.githubusercontent.com/franciscomirri90/Icone/main/consumi/consumi-favicon-64.png';
// doGet: HtmlService.createTemplateFromFile('Index').evaluate().setFaviconUrl(ICONA_URL)
```

### babysitter/ (Babysitter Leo)
- `babysitter-icon.svg`: icona completa (muso di leoncino con la criniera arancio, su fondo blu notte come l'app)
- `babysitter-mark.svg`: solo il leoncino, senza fondo
- `babysitter-icon-32.png`, `-64.png`, `-192.png`, `-512.png`: PNG ricavati dall'SVG
- `favicon.ico`: 16, 32, 48 e 64 px
- `babysitter-favicon-32.png`, `babysitter-favicon-64.png`: solo il leoncino, senza fondo, per la scheda del browser

Uso in Apps Script (`Code.gs` di App-Babysitter):

```js
const ICONA_URL = 'https://raw.githubusercontent.com/franciscomirri90/Icone/main/babysitter/babysitter-favicon-64.png';
// doGet: .setFaviconUrl(ICONA_URL) sulla pagina dell'app e su quella degli errori
```

### soldi/ (SOLDI, budget personale)
- `soldi-icon.svg`: icona completa (simbolo dell'euro: arco verde del disponibile, barre blu e corallo come
  "In arrivo" e "Ancora da spendere" nell'app, su fondo grafite come l'app)
- `soldi-mark.svg`: solo il simbolo, senza fondo
- `soldi-icon-32.png`, `-64.png`, `-192.png`, `-512.png`: PNG ricavati dall'SVG
- `favicon.ico`: 16, 32, 48 e 64 px
- `soldi-favicon-32.png`, `soldi-favicon-64.png`: solo il simbolo, senza fondo, per la scheda del browser

Uso in Apps Script (`Code.gs` di AppCasa_Soldi):

```js
var ICONA_URL = 'https://raw.githubusercontent.com/franciscomirri90/Icone/main/soldi/soldi-favicon-64.png';
// doGet: .setFaviconUrl(ICONA_URL)
```

Non rinominare né spostare i file usati dalle app: l'URL è scritto nel loro codice.
