FROM node:24-alpine

WORKDIR /app
RUN mkdir /feh-battles
COPY  ./feh-battles /feh-battles
COPY ./feh-server /feh-server
WORKDIR /feh-server
RUN npm ci --force
EXPOSE 3800

CMD ["npm", "start"]