FROM --platform=linux/amd64 node:16

WORKDIR /src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3001

CMD ["npm","start"]