FROM node:18-alpine
WORKDIR /app

COPY package.json package.json
COPY package-lock.json package-lock.json
RUN npm install

COPY . .

EXPOSE 8088/tcp
CMD ["node", "server.js"]