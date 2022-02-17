FROM node:16-alpine

# Added because of a bug with create react app and docker
ENV CI=true

WORKDIR /app
COPY package.json ./
RUN npm install
COPY ./ ./

CMD ["npm", "start"]