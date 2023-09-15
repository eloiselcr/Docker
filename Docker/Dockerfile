# Utilisez l'image officielle Node.js version 10
FROM node:10

# Copiez le contenu de votre application dans le conteneur
ADD . /app/

# Définissez le répertoire de travail
WORKDIR /app

# Installez les dépendances de votre application
RUN npm install
RUN npm install sqlite3 --save

# Exposez le port 2368 (assurez-vous que votre application utilise ce port)
EXPOSE 2368

# Définissez un volume pour les logs de l'application
VOLUME /app/logs

# Commande par défaut pour exécuter votre application
CMD npm run start
