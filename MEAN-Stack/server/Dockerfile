FROM node:latest

# Create app directory
RUN mkdir -p /opt/app
WORKDIR /opt/app
COPY package.json /opt/app/

RUN ["npm", "install"]

# Bundle app source
COPY . /opt/app

WORKDIR /opt/app

EXPOSE 3000
CMD [ "npm", "start" ]