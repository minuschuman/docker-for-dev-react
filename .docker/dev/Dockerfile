# Dockerfile
FROM node:current-alpine

WORKDIR /react-app
 
COPY ./package.json .
# COPY ./ ./

ENV PATH /app/node_modules/.bin:$PATH

RUN npm install

ENV PORT 3009
# EXPOSE 3009
CMD ["npm","run", "start"]