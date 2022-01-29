# Specify the base image
FROM node:alpine

# Setup the working directory
WORKDIR /app/usr

# Cache package.json file
COPY ./package.json ./

# Install dependencies
RUN npm install

# Copy remaining project files
COPY ./ ./

# Run startup command
CMD [ "npm", "start" ]
