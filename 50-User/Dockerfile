FROM node:20
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV mongo="true" \
    mongo_url="mongodb://mongodb:27017/catalogue" \
    redis_url="redis://redis:6379"
CMD ["node", "server.js"]

