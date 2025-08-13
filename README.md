# CollegeBook (Fork – Hugo Verly) Please run from Mergeing branch

> Fork de [CollegeBook](https://github.com/hugovrl29/CollegeBook) orienté **UX des événements** et **gestion des sièges**.

## 🎯 Objectif du fork
Mettre en avant mes contributions front/back : affichage des événements, et logique de sélection de sièges (groupes VIP, couleurs, états).

## 🧩 Principales contributions
- **Events page (cards)** : layout
- **Seat management (vanilla JS)** :
  - Groupes personnalisables (ex. `VIP`, `VIP2`, etc.)
  - Codes couleur : `disponible`, `vendu`, `sélectionné`, `VIP`, `VIP2`
  - Règles de sélection et retour visuel en temps réel
  - Animation *hover* en JS
- **Django** : vues/urls nécessaires au flux events et réservation

## 🛠️ Stack
- **Backend** : Python / Django
- **Frontend** : JavaScript (vanilla) + CSS
- **Paiement** : Stripe (Test)
- **DB** : SQLite (dev)

## 🚀 Lancer en local
```bash
git clone https://github.com/hugovrl29/CollegeBook
python -m venv .venv && source .env/bin/activate   # Windows: .env\Scripts\activate
pip install -r requirements.txt
sh restore_BD.sh
python ./src/manage.py runserver
