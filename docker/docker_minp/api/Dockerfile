# api/Dockerfile
FROM python:3.8-buster

MAINTAINER Votre Nom <beaugrand.axel@gmail.com>

# Mise à jour et installation des dépendances système
RUN apt update -y && apt install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y

# Copie des fichiers nécessaires
COPY requirements.txt /requirements.txt
COPY student_age.py /student_age.py

# Installation des dépendances Python
RUN pip3 install -r /requirements.txt

# Création du volume pour les données persistantes
VOLUME ["/data"]

# Exposition du port
EXPOSE 5000

# Commande de démarrage
CMD ["python3", "./student_age.py"]