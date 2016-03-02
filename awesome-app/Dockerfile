FROM node:onbuild

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY package.json /usr/src/app
RUN npm install

COPY index.js /usr/src/app

ENV PORT 8080

EXPOSE ${PORT}
CMD ["npm", "start"]
