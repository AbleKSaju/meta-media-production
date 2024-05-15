# Use a specific version of Node.js
FROM --platform=linux/amd64 node:18


# Set the working directory in the container
WORKDIR /app

# Copy only the package.json and package-lock.json to leverage Docker cache
COPY package*.json ./


# Install dependencies using Yarn
RUN yarn install --force

# Copy the entire project files to the working directory
COPY . .

# Expose the port your app runs on (in Vite, it's typically 3000 during development)
EXPOSE 5173

# Specify the command to run your application (for local development)
CMD ["npm", "run", "dev"]