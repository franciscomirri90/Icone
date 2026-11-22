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

Uso in Apps Script (`Code.gs`):

```js
const ICONA_URL = 'https://raw.githubusercontent.com/franciscomirri90/Icone/main/consumi/consumi-icon-64.png';
// doGet: HtmlService.createTemplateFromFile('Index').evaluate().setFaviconUrl(ICONA_URL)
```

Non rinominare né spostare i file usati dalle app: l'URL è scritto nel loro codice.
