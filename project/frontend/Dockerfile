FROM node:12.19.0-buster

RUN mkdir /usr/app
WORKDIR /usr/app

COPY ./package.json /usr/app
COPY ./package-lock.json /usr/app
RUN npm install --silent

COPY . /usr/app

EXPOSE 3000

CMD ["npm", "start"]
