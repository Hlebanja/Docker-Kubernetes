# Use an existing docker image as a base
FROM node:alpine
WORKDIR /usr/app

# Download and install a dependency
    # alternatively, we could use an image from someone who has done an image with pre installed node and npm
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Tell the image what to do when it starts as a container
CMD ["npm", "start"] 