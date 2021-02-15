FROM alpine:3.12.0

ADD ./src/go/main.go .

RUN apk update && apk add go && go build main.go && apk del go

CMD ["/main"]