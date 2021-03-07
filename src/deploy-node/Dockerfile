FROM node:latest

RUN mkdir /usr/src/node
WORKDIR /usr/src/node
COPY . /usr/src/node

RUN npm install

RUN npm install -g typescript
RUN tsc

EXPOSE 3000
#CMD ["sleep", "3600"]
CMD ["npm", "run", "start"]