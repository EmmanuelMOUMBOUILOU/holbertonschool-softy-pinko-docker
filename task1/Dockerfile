# Utilise l’image Ubuntu la plus récente comme base
FROM ubuntu:latest

# Met à jour APT et met à jour les paquets installés
RUN apt-get update && apt-get upgrade -y

# Installer Python3 et pip3
RUN apt-get install -y python3 python3-pip

# (Optionnel) Supprimer le blocage "externally managed"
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Installer Flask via pip
RUN pip3 install flask

# Définir le répertoire de travail
WORKDIR /app

# Copier ton code dans l'image
COPY ./api.py /app/api.py

# Lancer le serveur Flask
CMD ["python3", "api.py"]
