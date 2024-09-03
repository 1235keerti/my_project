# Use the official Node.js image from the Docker Hub 
FROM node:20 
ECHO is on.
# Set the working directory in the container 
WORKDIR /app 
ECHO is on.
# Copy the package.json and package-lock.json into the container 
COPY package*.json ./ 
ECHO is on.
# Install the Node.js dependencies 
RUN npm install 
ECHO is on.
# Copy the rest of the application code into the container 
COPY . . 
ECHO is on.
# Expose the port the app runs on 
EXPOSE 3000 
ECHO is on.
# Command to run the Node.js app 
CMD ["npm", "start"] 
