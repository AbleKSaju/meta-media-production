FROM --platform=linux/amd64 node:16

WORKDIR /src/app

COPY package*.json ./

RUN npm install

RUN npm install -g nodemon

COPY . .

EXPOSE 3003

CMD ["npm","start"]