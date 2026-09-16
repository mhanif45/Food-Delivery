FROM node:18-slim

WORKDIR /app

# Install python and build tools for native node modules
RUN apk add --no-cache python3 make g++

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 4000

CMD ["npm", "start"]
