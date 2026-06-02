# Base Image
FROM node:alpine

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
