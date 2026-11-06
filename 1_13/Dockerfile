FROM golang:1.16-alpine

WORKDIR /mybackend

COPY . ./

RUN go build

CMD ["./server"]
