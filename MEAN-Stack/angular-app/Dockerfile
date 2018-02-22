FROM node:6.9.0
# Create app directory
RUN mkdir -p /opt/app
WORKDIR /opt/app
COPY package.json /opt/app/

RUN ["npm", "install"]

# Bundle app source
COPY . /opt/app

EXPOSE 4200/tcp
CMD [ "npm", "start", "--", "--host", "0.0.0.0" ]