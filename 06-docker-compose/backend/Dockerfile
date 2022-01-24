FROM node:lts

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 8000

VOLUME [ "backend-logs:/app/logs" ]

VOLUME [ "/app/node_modules" ]

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

CMD [ "npm", "start" ]