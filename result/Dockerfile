FROM node:8.16.0-alpine

WORKDIR /app 

COPY package.json package.json

RUN npm install  && \ 
    npm audit fix 

COPY . . 

EXPOSE 4000

CMD ["npm", "start"] 
