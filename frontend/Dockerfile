FROM node:18-alpine

WORKDIR /app

# add '/app/node_modules/.bin' to $PATH
ENV PATH /app/node_modules/.bin:$PATH
# install application dependencies
COPY package*.json ./
#RUN npm install -g npm@latest
RUN npm install
# RUN npm install react-scripts -g

# copy app files
COPY . .

EXPOSE 3000
CMD ["npm", "start"]
