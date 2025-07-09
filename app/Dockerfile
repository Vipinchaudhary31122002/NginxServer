FROM node:22-alpine

# Set working directory
WORKDIR /app

COPY package.json .
COPY package-lock.json .

# Install dependencies (only if needed)
RUN npm install

# Copy app files
COPY . .

# Expose the port your Node.js app will use
EXPOSE 3000

# Start the app
CMD npm install && node server.js