FROM node:12-alpine

COPY . ./client/
WORKDIR /client

RUN npm install
RUN npm run build

EXPOSE 8080

CMD ["sh", "-c", "npm run start"]
