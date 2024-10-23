 # Utiliser une image Python comme base
FROM python:3.9-slim

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le fichier requirements.txt dans le conteneur
COPY requirements.txt requirements.txt

# Installer les dépendances
RUN pip install -r requirements.txt

# Copier le reste du code de l'application dans le conteneur
COPY app.py app.py

# Exposer le port 5000
EXPOSE 5000

# Commande pour exécuter l'application Flask
CMD ["python", "app.py"]

