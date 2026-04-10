# Codice sconto SempreFarmacia, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto SempreFarmacia** da [shopilo.it](https://shopilo.it/negozi/semprefarmacia.it). Restituisce **coupon SempreFarmacia** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-semprefarmacia](https://shopilo-it.github.io/codice-sconto-semprefarmacia/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-semprefarmacia
cd codice-sconto-semprefarmacia
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "SempreFarmacia",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su prodotti per la salute",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/semprefarmacia.it"
  }
]
```

## Coupon SempreFarmacia disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su prodotti per la salute | [shopilo.it](https://shopilo.it/negozi/semprefarmacia.it) |

Codici attivi: **[shopilo.it/negozi/semprefarmacia.it](https://shopilo.it/negozi/semprefarmacia.it)**

## Domande frequenti

### Come utilizzo un codice sconto SempreFarmacia?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/semprefarmacia.it), aggiungi i prodotti al carrello su SempreFarmacia e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon SempreFarmacia?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher SempreFarmacia piu recenti?
La pagina [shopilo.it/negozi/semprefarmacia.it](https://shopilo.it/negozi/semprefarmacia.it) viene aggiornata quotidianamente con i codici sconto SempreFarmacia, voucher SempreFarmacia e coupon promozionali SempreFarmacia piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su SempreFarmacia

SempreFarmacia e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/semprefarmacia.it) trovi i migliori codici sconto SempreFarmacia, coupon SempreFarmacia verificati e voucher SempreFarmacia attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-semprefarmacia
```

```javascript
const { fetchCoupons } = require('codice-sconto-semprefarmacia');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
