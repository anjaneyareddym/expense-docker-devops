FROM node:20
EXPOSE 8080
#TO GET THE NAME OF THE CONTINER
#WE AHVE TO GIVE THE CONTAINER NAME
# docker run -d --name mysql mysql:v1
ENV DB_HOST="mysql"
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
CMD ["node","index.js"]     

