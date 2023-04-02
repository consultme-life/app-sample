FROM node:13.13.0-alpine3.10
LABEL "maintainer"="kk@g.com"
WORKDIR /code
COPY package*.json .
RUN npm install --no-optional && npm cache clean --force
COPY . .
ENV PATH /code/node_modules/.bin:$PATH
EXPOSE 5000
ENTRYPOINT ["npm", "start"]