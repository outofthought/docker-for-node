
FROM node:10.22.1-stretch

RUN  apt-get update && apt-get install -y graphicsmagick

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

ENV CHARCOAL_FACTOR=0.1

CMD ["node", "index.js"]