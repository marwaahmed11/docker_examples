FROM node:latest

WORKDIR /nodeapp

COPY nodeapp /nodeapp

RUN npm install

EXPOSE 3000

CMD ["node", "/nodeapp/app.js"]
