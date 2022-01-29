# Specific the base image
FROM node:alpine

# Specific the working directory
WORKDIR /usr/app

# Copy the package.json file first to cache the changes
COPY ./package.json ./

# Copy remaining files
COPY ./ ./

# Install some dependencies
RUN npm install

# Default command to run on container startup.
CMD [ "npm", "start" ]
