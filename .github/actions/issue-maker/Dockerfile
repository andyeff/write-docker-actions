FROM node:slim
COPY package*.json ./
RUN npm install
RUN cat /root/.npm/_logs/*
COPY . .
CMD [ "node", "/src/index.js" ]
