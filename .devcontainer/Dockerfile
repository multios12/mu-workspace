FROM node:24.16.0-alpine
RUN apk  --no-cache --update add go git tzdata  poppler poppler-utils poppler-data libwebp-dev && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apk del tzdata && \
    go install -v golang.org/x/tools/gopls@latest && \
    go install -v github.com/go-delve/delve/cmd/dlv@latest && \
    go install -v honnef.co/go/tools/cmd/staticcheck@latest

COPY ./package.json ./yarn.lock ./
