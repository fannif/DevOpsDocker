FROM golang

WORKDIR /usr/src/app

RUN export PATH=$PATH:/usr/local/go/bin

COPY ./example-backend .

ENV REQUEST_ORIGIN=http://localhost:5000

RUN go build

EXPOSE 8080

CMD ["./server"]
