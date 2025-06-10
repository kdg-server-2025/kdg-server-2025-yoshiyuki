FROM golang:1.16 AS build

# 作業ディレクトリの指定
WORKDIR /app

COPY main.go .

RUN go build main.go

FROM alpine:3.22 AS run

# --fromは一つ目のステージを指定.
COPY  --from=build app/ .

CMD ["/main"]
