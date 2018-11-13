FROM clojure:lein-alpine
LABEL maintainer="Shogo Ohta <athos0220@gmail.com>"

ENV CLI_VERSION=1.9.0.397

RUN echo '@testing http://dl-cdn.alpinelinux.org/alpine/edge/testing' >> /etc/apk/repositories \
 && apk add --update --no-cache bash curl rlwrap@testing nodejs-current \
 && wget https://download.clojure.org/install/linux-install-$CLI_VERSION.sh \
 && chmod +x linux-install-$CLI_VERSION.sh \
 && ./linux-install-$CLI_VERSION.sh
