# About Image: Use LTS version for maintenance purpose and use alpine to reduce image size.
FROM node:10-alpine

LABEL vendor="Dynamic Lab"
LABEL maintainer="pangxiaoxi@gmail.com, cndream@gmail.com, daiyiyi1991@gmail.com"
LABEL description="dv-ingestor dev docker image"

ARG DEV_HOME
ENV APP_HOME $DEV_HOME/app

WORKDIR $APP_HOME

# run npm install at CMD level, so that we don't need to build new images again and again
CMD npm install --quiet &&\
    npm run debug