FROM node:14.17.0
ENV NODE_ENV=production

# Create /usr/app directory
WORKDIR /usr/app

# Install dependencies
COPY package*.json .
COPY package-lock.json .
RUN npm install --production --quiet

# Copy source files
COPY . .

# Run the app
CMD ["npm", "start"]