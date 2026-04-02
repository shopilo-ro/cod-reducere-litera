# Cod reducere Litera — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Litera** de pe [shopilo.ro](https://shopilo.ro/magazin/litera.ro). Returneaza **cupoane Litera** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-litera](https://shopilo-ro.github.io/cod-reducere-litera/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-litera
cd cod-reducere-litera
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Litera",
    "code": "SHOPILO10",
    "discount": "10 lei",
    "description": "10 lei reducere la orice produs",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/litera.ro"
  }
]
```

## Cupoane Litera disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10 lei | 10 lei reducere la orice produs | [shopilo.ro](https://shopilo.ro/magazin/litera.ro) |

Codurile active: **[shopilo.ro/magazin/litera.ro](https://shopilo.ro/magazin/litera.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Litera?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/litera.ro), adauga produsele in cos pe Litera, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Litera?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Litera?
Pagina [shopilo.ro/magazin/litera.ro](https://shopilo.ro/magazin/litera.ro) este actualizata zilnic cu cele mai noi cod reducere Litera, voucher Litera si cupon promotional Litera.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Litera

Litera este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/litera.ro) cele mai bune cod reducere Litera, cupoane Litera verificate si voucher Litera active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-litera
```

```javascript
const { fetchCoupons } = require('cod-reducere-litera');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
