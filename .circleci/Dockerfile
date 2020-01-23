FROM alpine:3.7
RUN apk add --update nginx && touch /build-2.0 && mkdir -p /run/nginx && touch /index.html
COPY activesupport-4.2.1.gem /
COPY utils.js /
COPY default.conf /etc/nginx/conf.d/
CMD ["nginx", "-g", "daemon off;"]
