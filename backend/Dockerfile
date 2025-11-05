FROM node:20
WORKDIR /opt/backend
COPY package.json .
COPY *.js .
RUN npm install
ENV db_host=mysql
CMD ["node", "index.js"]
