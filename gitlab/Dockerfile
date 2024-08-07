FROM nginx:1.21.1-alpine

LABEL maintainer="Beaugrand Axel"

RUN apk update && \
    apk add --no-cache git && \
    rm -rf /var/cache/apk/* && \
    rm -rf /usr/share/nginx/html/* && \
    git clone https://github.com/diranetafen/static-website-example.git /usr/share/nginx/html && \
    rm -rf /usr/share/nginx/html/.git

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
