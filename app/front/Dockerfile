FROM nginx:alpine

RUN apk add --no-cache bash

COPY entrypoint.sh .
RUN chmod +x entrypoint.sh

COPY . /usr/share/nginx/html/

ENTRYPOINT ["/entrypoint.sh"]