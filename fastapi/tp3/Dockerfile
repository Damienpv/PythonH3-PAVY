FROM tiangolo/uvicorn-gunicorn-fastapi:python3.11-slim

WORKDIR /app

# Copier le contenu du dossier app dans /app
COPY ./app /app

# Copier le fichier requirements.txt à la racine dans le conteneur
COPY requirements.txt .

# Installer les dépendances
RUN pip install --no-cache-dir -r /app/requirements.txt

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]
