FROM node:12-alpine

COPY . ./api/
WORKDIR /api

RUN npm ci
RUN npm i -g pm2
RUN npm run build

EXPOSE 3000

#CMD ["pm2-runtime", "start", "--name", "'jira_api'", "node", "--", "-r", "./tsconfig-paths.js", "build/index.js"]
CMD ["sh", "-c", "npm run start"]