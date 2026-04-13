# Code promo i-Run, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo i-Run** depuis [shopilo.fr](https://shopilo.fr/reductions/i-run.fr). Renvoie les **coupons i-Run** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-i-run](https://shopilo-fr.github.io/code-promo-i-run/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-i-run
cd code-promo-i-run
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "i-Run",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur les chaussures de running",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/i-run.fr"
  }
]
```

## Coupons i-Run disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur les chaussures de running | [shopilo.fr](https://shopilo.fr/reductions/i-run.fr) |

Codes actifs : **[shopilo.fr/reductions/i-run.fr](https://shopilo.fr/reductions/i-run.fr)**

## Questions frequentes

### Comment utiliser un code promo i-Run ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/i-run.fr), ajoutez les produits a votre panier sur i-Run et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons i-Run ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction i-Run les plus recents ?
La page [shopilo.fr/reductions/i-run.fr](https://shopilo.fr/reductions/i-run.fr) est mise a jour quotidiennement avec les codes promo i-Run, bons de reduction i-Run et coupons promotionnels i-Run les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de i-Run

i-Run est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/i-run.fr), retrouvez les meilleurs codes promo i-Run, coupons i-Run verifies et bons de reduction i-Run actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-i-run
```

```javascript
const { fetchCoupons } = require('code-promo-i-run');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
