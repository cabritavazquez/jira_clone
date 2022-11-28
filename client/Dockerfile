FROM node:12-alpine

ENV API_URL=http://api.default.svc.cluster.local:3000

COPY . ./client/
WORKDIR /client

RUN npm install
RUN npm run build

EXPOSE 8080

CMD ["sh", "-c", "npm run start"]
