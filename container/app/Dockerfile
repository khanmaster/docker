
FROM node:latest

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

COPY provision.sh /
RUN /provision.sh && /provision.sh 

#ENTRYPOINT [ "/provision.sh"]

CMD ["node", "app.js"]

