FROM node:14

# which files that live here on our local machine go to image
# dot 1 is folder is contains docker file (src)
# dot 2 is path inside of the image in image ()host file system image/container file system (dest)
# COPY . . <src> <dest>
# COPY . .
# COPY . /app (กำหนดให้ตรง WORKDIR)
# WORKDIR /app ใช้ก่อน COPY

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

# explain for to know this app is listening in port (unnecessary)
EXPOSE 80

# RUN node server.js
CMD ["node", "server.js"]
