FROM node:alpine

WORKDIR /usr/app

# this command says, do the run npm step, only if there is a 
# change in the package.json file, otherwise use caches.
COPY ./package.json ./ 
RUN npm install
COPY ./ ./ 

CMD ["npm", "start"] 