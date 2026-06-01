
# Specify a base image 
FROM node:14-alpine

# Define working directory
WORKDIR /usr/app

# Install some dependencies
COPY ./package.json ./
RUN npm install

COPY ./ ./

# Default command to run
CMD ["npm", "start"]