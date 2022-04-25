FROM node:12-alpine

RUN mkdir /app

WORKDIR /app

COPY package.json /app/
COPY package-lock.json /app/

RUN npm install

COPY . .

# ENV PORT=5001
EXPOSE 5001

CMD [ "npm", "start" ]