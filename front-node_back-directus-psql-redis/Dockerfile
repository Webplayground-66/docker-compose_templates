# image
FROM node:16
# nom du dossier de l'app
WORKDIR /mon_dossier
COPY /package.json ./
RUN npm install
COPY . .
# port d'écoute
EXPOSE 3500
CMD ["npm", "start"]