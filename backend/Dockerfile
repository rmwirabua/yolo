FROM node:12-alpine

RUN mkdir /app

WORKDIR /app

COPY package.json /app/
COPY package-lock.json /app/

RUN npm install

COPY . .

# ENV PORT=5000

EXPOSE 5000

CMD [ "npm", "start" ]