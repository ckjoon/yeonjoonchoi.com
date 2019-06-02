

# base image
FROM node:11.12.0-alpine as builder

# set working directory
WORKDIR /usr/src/app

# install app dependencies
ENV PATH /usr/src/app/node_modules/.bin:$PATH
COPY package.json /usr/src/app/package.json

RUN npm install
RUN npm install -g @angular/cli

# create build
COPY . /usr/src/app
# start app
CMD ng serve --host 0.0.0.0
