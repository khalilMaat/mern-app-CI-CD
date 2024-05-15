#Dockerfile of express app
#base image
FROM node:20-alpine

RUN echo "Dockerfile of express app"

#owner
LABEL author="khalil maatoug"

#work dir
WORKDIR /app

#copy package file to workdir
COPY package*.json ./app

#install node modules
RUN npm install

#Copy ofther file of project to /app
COPY . ./app

#Run the app
CMD ["npm","run","dev"]

EXPOSE 5000






