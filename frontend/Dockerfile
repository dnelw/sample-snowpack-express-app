FROM node:14.15.3

ENV FRONTEND_PORT=${FRONTEND_PORT:-8080}

EXPOSE ${FRONTEND_PORT}

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

CMD npm run serve
