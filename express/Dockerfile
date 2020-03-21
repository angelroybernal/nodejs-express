FROM node:12-stretch
MAINTAINER angelroybernal

RUN DEBIAN_FRONTEND=noninteractive && \
apt-get update \
&& apt-get upgrade -yq

RUN npm install express --save
COPY ./app /opt/js

EXPOSE 3000

CMD ["/usr/local/bin/node","/opt/js/index.js"]
