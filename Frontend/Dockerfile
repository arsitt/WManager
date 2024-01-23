# Use an official Node runtime as a parent image
FROM node:18.13

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the application files to the working directory
COPY . .

# Make port 80 available to the world outside this container
EXPOSE 4200

# Define environment variable
ENV NAME World

# Run app when the container launches
CMD ["npm", "start"]
