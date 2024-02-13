# Use the official Node.js 20 as a parent image
FROM node:20

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json (if available) to the working directory
# COPY package*.json ./
COPY package.json .

# Install project dependencies
RUN npm install

# Copy the rest of your Vue.js application's source code to the working directory
COPY . .

# # Make port 5173 available to the world outside this container
EXPOSE 5173

# # Command to run the Vue.js development server
CMD ["npm", "run", "dev"]
