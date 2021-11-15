FROM node:14.18.1-alpine

WORKDIR /src/webapp

EXPOSE 3001

COPY . .

RUN npm install express --save

ENTRYPOINT ["node"]

CMD ["my-app.js"]