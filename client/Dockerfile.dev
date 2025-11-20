FROM node:25-alpine

WORKDIR /app

# install dependencies only
COPY ./package.json ./
RUN npm install

# copy the rest of the app. It allows to cache dependencies
COPY . .

CMD ["npm", "run", "start"]