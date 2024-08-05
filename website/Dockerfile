# Frontend Dockerfile
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package.json package-lock.json ./

RUN npm ci

# Copy application code
COPY . .


# Expose port
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]