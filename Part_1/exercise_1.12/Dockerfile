# Install node 16 major version.
FROM node:16.20.2

EXPOSE 5000

WORKDIR /usr/src/app

# Copy only dependency info
COPY package* ./

# Install packages
RUN npm install

# Copy rest of files
COPY . .

# Build static files
RUN npm run build

# Install serve
RUN npm install -g serve

CMD [ "serve", "-s", "-l", "5000", "build" ]