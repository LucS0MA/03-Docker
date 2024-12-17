FROM node:lts-alpine

WORKDIR /app

COPY index.html index.html
COPY package*.json ./
RUN npm install

COPY ./src/main.tsx ./src/main.tsx
COPY vite.config.ts vite.config.ts
COPY src src
COPY public public

CMD npm run dev