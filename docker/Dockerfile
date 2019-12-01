FROM alpine
EXPOSE 8080

RUN apk add --no-cache php-cli php-mysqli php-session php7-pecl-memcached && mkdir /app

COPY . /app

WORKDIR /app
ENTRYPOINT ["php", "-S", "0.0.0.0:8080", "-t"]
CMD ["/app"]
