# Use the official Node.js Image
FROM node:20-alpine as BUILD_IMAGE

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json for the server
COPY package*.json ./
RUN npm i

# Copy the rest of the application source code to the container
COPY . .

# Expose the port on which your server will listen
EXPOSE 5000

# Start the server
CMD ["npm", "run", "dev"]
