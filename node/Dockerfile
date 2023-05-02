FROM node:15

WORKDIR /usr/src/app

RUN apt-get install -y wget
ENV DOCKERIZE_VERSION v0.6.1
RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && tar -C /usr/local/bin -xzvf dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && rm dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz

# Other way for wait-for-it containers, it's use the wait-for project https://github.com/eficode/wait-for

EXPOSE 3000

# CMD [ "node", "index.js" ]
