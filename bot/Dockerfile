# Utiliser une image de base Python officielle
FROM python:3.9-slim

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le fichier requirements.txt dans le répertoire de travail
COPY requirements.txt .

# Installer les dépendances Python
RUN pip install --no-cache-dir -r requirements.txt

# Copier tout le contenu du projet dans le répertoire de travail
COPY . .

# Exposer le port sur lequel votre application va fonctionner
EXPOSE 5000

# Définir la commande par défaut pour exécuter l'application
CMD ["python", "main.py"]
