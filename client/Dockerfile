# Use the official Node.js image as the base image
FROM node:14

# Create the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies, including nodemon
RUN npm install -g nodemon

# Copy the entire server directory to the container
COPY . .

# Expose port 5000
EXPOSE 5000

# Command to run the application
CMD ["npm", "start"]

