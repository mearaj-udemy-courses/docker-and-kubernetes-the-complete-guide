# Specify a base file
FROM node:alpine

# If app directory doesn't exist, it will be created
# and the program will run inside /usr/app
WORKDIR /usr/app

# Install some dependencies
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Default command
CMD [ "npm","start"]