FROM node:alpine

ENV CI=true

WORKDIR /app
COPY package.json ./
ENV NODE_OPTIONS --openssl-legacy-provider
RUN npm install
COPY ./ ./ 

CMD ["npm", "start"]