FROM node:16-alpine

RUN apk update && apk add git

WORKDIR /app
RUN git clone https://github.com/docker-hy/material-applications.git

WORKDIR /app/material-applications/example-frontend
# RUN npm install -g serve
RUN npm install
# CMD serve -s -l 5000 build
CMD ["npm", "start"]


