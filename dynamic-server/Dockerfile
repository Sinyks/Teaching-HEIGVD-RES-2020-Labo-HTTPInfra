FROM node:lts

COPY src/ /opt/app

WORKDIR /opt/app

# génère les dépendance à l'intérieur du container
RUN npm install

EXPOSE 3000

CMD ["node","index.js"]
