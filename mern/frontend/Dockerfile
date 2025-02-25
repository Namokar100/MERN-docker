FROM node:18.9.1

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev"]


##How to run the Dockerfile

# docker ps --> to check docker is active or not, if not open docker desktop
# docker build -t mern-frontend . --> to build the docker image
# docker network create mern --> to create a network
# docker run -d --network mern --name mongodb mongo --> to run the mongodb
# docker run --network=mern --name mongodb -d -p 27017:27017 -v ~/ongo:latest --> to run the mongodb
# docker build -t mern-backend . --> to build the backend image
# docker run -d --network mern --name mern-backend mern-backend --> to run the backend
# docker logs backend --> to check the logs of the backend