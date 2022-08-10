FROM node:16.16.0

WORKDIR /app

ENV LANG C.UTF-8
ENV TZ Asia/Tokyo
ENV HOST 0.0.0.0

ADD package.json /app/package.json
ADD package-lock.json /app/package-lock.json

RUN apt-get update -y && \
  apt-get upgrade -y && \
  npm install npm && \
  npm install ejs &&\
  npm install nuxt &&\
  npm install create-nuxt-app &&\
  npm install defu &&\
  npm i vue

ADD . /app

RUN npm run build

EXPOSE 3000

CMD ["npm", "run", "start"]
