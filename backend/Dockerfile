FROM node

WORKDIR /app

COPY package.json .

RUN npm install

ENV USERNAME=root
ENV PASSWORD=root

COPY . .

EXPOSE 80

CMD ["node", "app.js"]