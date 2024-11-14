FROM node:14-alpine

ENV CI=true
ENV WDS_SOCKET_PORT=0

WORKDIR /app
COPY package.json ./
RUN npm install --legacy-peer-deps
COPY ./ ./

CMD ["npm", "start"]