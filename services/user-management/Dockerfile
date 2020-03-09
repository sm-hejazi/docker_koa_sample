# Use Node v12.16 as the base image.
FROM node:12.16.1

#Set the working directory
WORKDIR /usr/app

# Copy everything in current directory to /server folder
ADD . /server

# Install dependencies
RUN cd /server; \
    npm install

EXPOSE 3000

# Run node 
CMD ["node", "/server/src/server.js"]