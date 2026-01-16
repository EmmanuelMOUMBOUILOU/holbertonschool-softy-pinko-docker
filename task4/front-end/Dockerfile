# Utiliser l’image Nginx officielle
FROM nginx:latest

# Copier les fichiers du front-end vers le dossier web de Nginx
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copier le fichier de configuration Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
