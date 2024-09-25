# Frontend Dockerfile

# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app

# Copy the current directory contents into the container
COPY . .

# Copy package.json and package-lock.json first to leverage Docker cache
COPY package*.json ./


# Install dependencies
RUN npm install

# Make port 8080 available to the world outside this container
EXPOSE 8080

# Run the app when the container launches
CMD ["node", "app.js"]

