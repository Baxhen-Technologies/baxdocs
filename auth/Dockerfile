FROM node:alpine
ENV CI=true

WORKDIR /app
COPY package.json .
RUN npm install --only=prod
COPY . .
RUN npm build

CMD ["npm", "start"]