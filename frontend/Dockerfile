FROM node:13.8.0-alpine3.10

WORKDIR /app
COPY ./app/package.json /app

RUN npm install --quiet

# this will be a volume inside the container
RUN mkdir -p node_modules