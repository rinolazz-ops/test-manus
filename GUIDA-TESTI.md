# Come modificare i testi del sito

I testi del sito NON sono nel file `index.html` tradizionale: il sito è un'app
React compilata, quindi tutto il testo vive nel file `assets/index-home-v2.js`
(codice minificato, da non toccare).

Per questo, in fondo a `index.html` ho aggiunto un blocco chiamato **TESTI**:
da lì puoi cambiare QUALSIASI testo del sito senza toccare il codice compilato.

## Istruzioni

1. Apri `index.html` con un editor di testo (Blocco note va bene).
2. Scorri fino al blocco:

```html
<script>
/* ============================================================
   MODIFICA DEI TESTI DEL SITO  (basta editare la lista TESTI)
   ...
   ============================================================ */
(function () {
  var TESTI = {
    // --- Esempi: togli il // all'inizio per attivarli ---
    // "Prenota Valutazione": "Prenota una visita",
    // "Il Metodo di Cura": "Come lavoro",
    // "+39 049 123 4567": "+39 049 999 9999"
  };
```

3. Per cambiare un testo, togli i `//` davanti all'esempio e sostituisci
   i tuoi testi, oppure aggiungi una riga nuova nel formato:

```
"testo attuale": "testo nuovo",
```

Regole:
- Il "testo attuale" va copiato ESATTAMENTE come appare sul sito
  (basta anche solo una parte distintiva della frase, non serve la frase intera).
- Funziona per titoli, paragrafi, voci di menu, pulsanti, telefono, email...
- Se cambi il numero di telefono (o l'email), viene aggiornato automaticamente
  anche il link "tel:" / "mailto:" per le chiamate.
- Salva il file e ricarica la pagina per vedere il risultato.

## Esempio

```js
var TESTI = {
  "Ritrova il tuo movimento,": "Torna a muoverti,",
  "Orari di Ricevimento": "Orari dello studio",
  "+39 049 123 4567": "+39 333 123 4567",
  "studio@valeriaferrazfisioterapia.it": "info@miosito.it"
};
```

## Dopo le modifiche

Ricarica su GitHub il solo file `index.html` (Add file → Upload files),
sovrascrivendo quello esistente.
