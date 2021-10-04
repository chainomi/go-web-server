#Using Alphine variant of golang - small image size. Which would improve performance on the cloud. 
FROM golang:1.16-alpine

#Specifying the value of "PORT" variable, which ties to code in main.go file
ENV PORT=3030


EXPOSE 3030

#Creating directory /go-run in container and copying contents of current directory into it
RUN mkdir /go-run
COPY . /go-run

# RUN go get -d -v ./...
# RUN go install -v ./...

WORKDIR /go-run/

RUN go build -o main .

CMD ["/go-run/main"]