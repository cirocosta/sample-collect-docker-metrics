FROM alpine

RUN apk add --no-cache socat

EXPOSE [ "2375" ]

ENTRYPOINT [ "socat", "TCP-LISTEN:2375,reuseaddr,fork", "UNIX-CONNECT:/var/run/docker.sock" ]
