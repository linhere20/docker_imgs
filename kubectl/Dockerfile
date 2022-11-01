FROM alpine:latest

RUN apk add --update -t deps curl

RUN curl -L https://storage.googleapis.com/kubernetes-release/release/v1.25.2/bin/linux/amd64/kubectl -o /usr/local/bin/kubectl && chmod +x /usr/local/bin/kubectl

RUN apk del --purge deps && rm /var/cache/apk/*

CMD ["/bin/sh"]

