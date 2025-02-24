# Use an official Node.js runtime as a parent image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 3000

# Define environment variables (optional, can also be set in docker-compose or runtime)
# ENV DB_CONNECT=your_mongodb_connection_string
# ENV JWT_SECRET=your_jwt_secret
# ENV GOOGLE_MAPS_API=your_google_maps_api_key

# Command to run the application
CMD ["node", "server.js"]