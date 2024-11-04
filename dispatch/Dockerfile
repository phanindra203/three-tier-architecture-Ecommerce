FROM golang:1.18

WORKDIR /go/src/app

COPY *.go .

RUN go mod init dispatch && go mod tidy
RUN go build -o dispatch .

# Command to run the application
CMD ["./dispatch"]
