FROM python:3.11-alpine

# Installer les dépendances système nécessaires pour psycopg2 et autres packages

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["flask", "run", "--host=0.0.0.0", "--port=5000"]
