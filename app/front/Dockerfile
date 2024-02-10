FROM nginx:alpine

RUN apk add --no-cache bash

COPY entrypoint.sh .
RUN chmod +x entrypoint.sh

COPY . /usr/share/nginx/html/

RUN apt-get update && apt-get install -y dos2unix && dos2unix entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]