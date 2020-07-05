# Use a lighter version of Node as a parent image
FROM node:12-alpine

# Set the working directory to /app
WORKDIR /app

# copy package.json into the container at /app
COPY package*.json /app/

# install dependencies
RUN npm install

# Copy the current directory contents into the container at /app
COPY . /app/

# Run the app when the container launches
CMD ["npm", "start"]
