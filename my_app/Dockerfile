FROM node:alpine
WORKDIR /my_app
ENV PATH /my_app/node_modules/.bin:$PATH
COPY package.json ./
COPY ../package-lock.json ./
RUN npm install
COPY .. ./
CMD ["npm", "start"]