#Docker file for react app
#base image
FROM node:20-alpine

RUN echo "Dockerfile React app"

#owner
LABEL author="Maatoug khalil"

#work dir
WORKDIR /app

#copy package file
COPY package*.json ./app

#install dependencies
RUN npm install

#copy all other file to workdir
COPY . .

#run the app
CMD ["npm","start"]

EXPOSE 3000



