FROM node:9.10-alpine
MAINTAINER "Jonathan Callahan" jonathan@mazamascience.com

####################
# See:  https://github.com/BretFisher/node-docker-good-defaults/blob/master/Dockerfile

# install dependencies and set path
WORKDIR /opt
COPY package.json package-lock.json* ./
RUN npm install && npm cache clean --force
ENV PATH /opt/node_modules/.bin:$PATH


