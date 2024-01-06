FROM node:14
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 5001
ENV NODE_PORT 80
CMD [ "node", "index.js" ]