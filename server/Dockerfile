# 1. Use an official Node.js runtime as the base image
FROM node:18

# 2. Set the working directory inside the container
WORKDIR /app

# 3. Copy the package.json and package-lock.json (if present) to install dependencies first
COPY package*.json ./

# 4. Install the dependencies
RUN npm install --production

# 5. Copy the rest of your application code to the working directory
COPY . .

# 6. Expose the port your app runs on (if it's port 3000)
EXPOSE 4000

# 7. Set the default command to run your app
CMD ["npm", "start"]
