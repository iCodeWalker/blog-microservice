# Base Image
FROM node:alpine

ENV CI=true
ENV WDS_SOCKET_PORT=0
ENV BROWSER=none

# Working directory
WORKDIR /app

# Copy only package.json
COPY package.json ./

# Install packages
RUN npm install

# Copy all the files
COPY ./ ./

# Start command
CMD ["npm", "start"]
