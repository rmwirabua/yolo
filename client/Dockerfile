FROM node:14.16.0-alpine3.13

RUN mkdir /app

WORKDIR /app

COPY package.json /app/
COPY package-lock.json /app/

RUN npm install

COPY . .

# ENV PORT=5001
EXPOSE 5001

CMD [ "npm", "start" ]