#  creates a layer from the node:14-alpine Docker image.
# AS development cause in docker-compose set target is development
FROM node:14-alpine AS development
ENV NODE_ENV development
WORKDIR /app
COPY package.json .
COPY yarn.lock .
RUN yarn install
# COPY adds files from your Docker client’s current directory.
COPY . .
EXPOSE 3000
# CMD specifies what command to run within the container.
CMD ["yarn", "dev"]