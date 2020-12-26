FROM node:14.15.3

ENV BACKEND_PORT=${BACKEND_PORT:-5000}

EXPOSE ${BACKEND_PORT}

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

CMD npm run start
