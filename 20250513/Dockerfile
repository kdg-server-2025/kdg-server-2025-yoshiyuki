FROM golang:alpine

# 作業ディレクトリの指定
WORKDIR /

COPY main.go /

RUN go build main.go

CMD ["/main"]