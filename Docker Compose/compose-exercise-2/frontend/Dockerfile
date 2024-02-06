FROM node:14.16.0-alpine3.13
WORKDIR /app
RUN chown -R node:node /app
USER node:node
COPY package*.json ./
# COPY package.json package-lock.json .
RUN npm cache clean --force
RUN npm i 
COPY . ./
EXPOSE 3000
# RUN chmod o-r package*.json

CMD [ "npm", "start"]