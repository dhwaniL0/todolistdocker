# Use an official Node.js runtime as a parent image
FROM node:18

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port that the backend listens on (typically 5000 or 8080)
EXPOSE 5000

# Start the backend service
CMD ["npm", "start"]
