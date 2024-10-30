# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the entire backend code to the working directory
COPY . .

# Expose the port on which the app will run (e.g., 5000)
EXPOSE 5000

# Specify the command to run the app
CMD ["node", "index.js"]