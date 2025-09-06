# Use official Node.js 22 image
FROM node:22-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .


# Expose backend port (now using 3000)
EXPOSE 3000

# Start the server (ensure your app listens on port 3000)
CMD ["node", "index.js"]