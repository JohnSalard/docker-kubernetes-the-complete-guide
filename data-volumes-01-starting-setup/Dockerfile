FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

ARG DEFAULT_PORT=80
ARG DEFAULT_MESSAGE=OLE
ARG DEFAULT_WORD


# Recommend
ENV PORT=${DEFAULT_PORT}
ENV MESSAGE=${DEFAULT_MESSAGE}
ENV WORD=${DEFAULT_WORD}

# Not Recommend
# ENV PORT 80


# EXPOSE 80
EXPOSE ${PORT}

# VOLUME [ "feedback","/app/feedback" ]
# VOLUME [ ".","/app" ]
# VOLUME [ "/app/temp" ]
# VOLUME [ "/app/node_modules" ]


# CMD ["node","server.js"]
CMD ["npm","start"]
