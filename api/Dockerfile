FROM node:16-alpine

# Nodemon is a tool that watches for changes in files and restarts the server
RUN npm install -g nodemon

WORKDIR /app

COPY package.json .

RUN npm install

# Copy the entire directory to the current directory
COPY . . 

EXPOSE 4000

CMD ["npm", "run", "dev"]