FROM node:14.16.0-alpine3.13

RUN mkdir /app

WORKDIR /app

COPY package.json /app/
COPY package-lock.json /app/

RUN npm install

COPY . .

# ENV PORT=5000

EXPOSE 5000

CMD [ "npm", "start" ]