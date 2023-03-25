# Go version
FROM golang:1.19.1-alpine
# Update & git install
RUN apk add --update && apk add git
# Create app directory
RUN mkdir /go/src/app
# Set working dir
WORKDIR /go/src/app
# Move host files to working dir
ADD ./cmd/main.go /go/src/app/
# Compile & Execute
CMD ["go", "run", "main.go"]
# Port setting
EXPOSE 8080
