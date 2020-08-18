FROM node:13.7-alpine3.10

ENV TOPICO=meu-topico
ENV HOST=0.0.0.0
ENV PORTA=9092
ENV WEBHOOK=https://outlook.office.com/webhook/235dfff5-db64-49d6-b68d-8e30a9e2078c@11dbbfe2-89b8-4549-be10-cec364e59551/IncomingWebhook/e3e02cb1356e49599c552530432624af/0eaa375e-b457-47d7-9870-519e14bb9e31
ENV CANAL=lab-consumidor
#ENV CANAL=lab-testes

WORKDIR /usr/src/app
COPY package.json ./
RUN npm install -g --silent
COPY . .

CMD [ "npm", "start" ]
