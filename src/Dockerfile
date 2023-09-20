# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose the port your Node.js app is listening on (e.g., 4000)
EXPOSE 4000

# Define the command to run your Node.js app (modify this based on your project)
CMD ["node", "server.js"]