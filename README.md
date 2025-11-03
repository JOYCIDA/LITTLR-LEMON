# 🍋 Système de Réservation Little Lemon

## 🏗️ Présentation du projet
Le **Système de Réservation Little Lemon** est une application web développée avec **Django** permettant la gestion des réservations dans un restaurant.  
Elle offre la possibilité aux clients de **réserver une table**, de **choisir une date et un créneau horaire**, et d’afficher toutes les réservations existantes sous forme dynamique.  

Ce projet a été réalisé dans le cadre du **cours de Développement Full Stack** sur Coursera afin de démontrer les compétences acquises en :
- Développement web back-end avec Django
- Intégration d’une base de données MySQL
- Utilisation de JavaScript pour les interactions dynamiques
- Gestion d’API et format JSON

---

## 🚀 Fonctionnalités principales
✅ Formulaire intuitif de réservation de tables  
✅ Sélecteur de date interactif (calendrier intégré)  
✅ Empêche les doubles réservations pour une même date et heure  
✅ Actualisation automatique des données lors du changement de date  
✅ Affichage en temps réel de toutes les réservations (au format JSON)  
✅ Connexion avec une base de données MySQL pour le stockage persistant  

---

## 🧩 Technologies utilisées
- **Back-end :** Django 5.x (Python)
- **Base de données :** MySQL
- **Front-end :** HTML5, CSS3, JavaScript
- **Environnement :** pipenv / virtualenv
- **Contrôle de version :** Git et GitHub

---

## ⚙️ Installation et exécution

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/JOYCIDA/LITTLR-LEMON.git
cd LITTLR-LEMON

2️⃣ Créer et activer l’environnement virtuel

python -m venv venv
venv\Scripts\activate     # (Windows)
source venv/bin/activate  # (Mac/Linux)

3️⃣ Installer les dépendances

pip install -r requirements.txt

4️⃣ Configurer la base de données MySQL

Dans le fichier settings.py, modifiez la section DATABASES avec vos identifiants MySQL :

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'reservations',
        'USER': 'root',
        'PASSWORD': 'votre_mot_de_passe',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}

5️⃣ Effectuer les migrations et lancer le serveur

python manage.py makemigrations
python manage.py migrate
python manage.py runserver

Accédez ensuite à l’application via :
👉 http://127.0.0.1:8000/
🧠 Fonctionnement de l’application

    Page “Book” (/book) : permet aux utilisateurs de remplir un formulaire avec leur prénom, la date et le créneau horaire de réservation.

    Page “Réservations” (/bookings) : affiche toutes les réservations existantes au format JSON.

    API interne :

        /bookings?date=YYYY-MM-DD → retourne les réservations pour une date précise.

💡 Exemple d’utilisation

Un restaurateur peut :

    Visualiser toutes les réservations du jour ou d’une date donnée.

    Empêcher les réservations multiples sur le même créneau.

    Gérer facilement la disponibilité des tables via une interface claire et fluide.

👩‍💻 Auteur

Développé par : MOUAHA JOYCE
📧 Email : mouahajoyce25@gmail.com

🌐 GitHub : https://github.com/JOYCIDA/LITTLR-LEMON
🏅 Licence

Ce projet est open-source et disponible sous la licence MIT License
.
📚 Remarques complémentaires

    Le projet utilise pipenv pour la gestion de l’environnement virtuel et des dépendances.

    Les dépendances principales incluent Django et mysqlclient.

    Le code source HTML, CSS et JS du site est fourni et adapté à partir du modèle “Little Lemon” officiel.
