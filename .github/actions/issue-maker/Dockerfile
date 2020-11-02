FROM node:slim
COPY package*.json ./
RUN npm cache clean --force
RUN npm install || cat /root/.npm/_logs/*
COPY . .
CMD [ "node", "/src/index.js" ]
