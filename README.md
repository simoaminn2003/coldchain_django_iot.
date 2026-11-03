# Projet Cold Chain - IoT & Django REST Framework

Application web et API REST pour la collecte, la sauvegarde et la visualisation en temps réel de données de température et d'humidité mesurées par une carte ESP8266 et un capteur DHT11.

## Fonctionnalités
- **API REST (DRF)** : Enregistrement (POST) et consultation (GET) des mesures au format JSON.
- **Tableau de bord Web** : Visualisation en temps réel (cartes + graphiques dynamiques Chart.js).
- **Système d'Alerte** : Notification Email (Gmail) et Telegram si température > 25°C.
- **Client ESP8266** : Envoi automatique des données toutes les 10 secondes.

## Installation
1. Extraire l'archive et ouvrir le dossier dans PyCharm / Terminal.
2. Créer l'environnement virtuel : `python -m venv .venv` puis l'activer.
3. Installer les dépendances : `pip install -r requirements.txt`
4. Appliquer les migrations : `python manage.py migrate`
5. Lancer le serveur : `python manage.py runserver 0.0.0.0:8000`
