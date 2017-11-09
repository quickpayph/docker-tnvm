# alinode-v3.8.0

## overview

* alinode-v3.8.0

* node v8.9.0

* npm 5.5.1

* cnpm 5.1.1

## environments

EXPOSE 80

WORKDIR /srv/nodejs


## run container

`docker run --name tnvmtest -d \
--restart \
-e "TZ=Asia/Shanghai" \
-e "NODE_ENV=production" \
-e "EGG_SERVER_ENV=prod" \
-v /root/vue-jd:/srv/nodejs \
-p 7001:80  \
gzlrs/tnvm`


## build image

docker build -t gzlrs/tnvm:alinode-v3.8.0  .


