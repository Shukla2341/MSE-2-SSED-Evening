
FROM node:20-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install production dependencies
RUN npm ci --omit=dev

# Copy backend application
COPY src ./src

# Backend port
EXPOSE 3000

# Start backend
CMD ["npm", "start"]
