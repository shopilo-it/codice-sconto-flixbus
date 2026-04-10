# Codice sconto FlixBus, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto FlixBus** da [shopilo.it](https://shopilo.it/negozi/flixbus.it). Restituisce **coupon FlixBus** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-flixbus](https://shopilo-it.github.io/codice-sconto-flixbus/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-flixbus
cd codice-sconto-flixbus
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "FlixBus",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su viaggi in autobus",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/flixbus.it"
  }
]
```

## Coupon FlixBus disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su viaggi in autobus | [shopilo.it](https://shopilo.it/negozi/flixbus.it) |

Codici attivi: **[shopilo.it/negozi/flixbus.it](https://shopilo.it/negozi/flixbus.it)**

## Domande frequenti

### Come utilizzo un codice sconto FlixBus?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/flixbus.it), aggiungi i prodotti al carrello su FlixBus e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon FlixBus?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher FlixBus piu recenti?
La pagina [shopilo.it/negozi/flixbus.it](https://shopilo.it/negozi/flixbus.it) viene aggiornata quotidianamente con i codici sconto FlixBus, voucher FlixBus e coupon promozionali FlixBus piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su FlixBus

FlixBus e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/flixbus.it) trovi i migliori codici sconto FlixBus, coupon FlixBus verificati e voucher FlixBus attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-flixbus
```

```javascript
const { fetchCoupons } = require('codice-sconto-flixbus');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
