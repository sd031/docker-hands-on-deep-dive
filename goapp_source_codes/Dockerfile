FROM golang:1.16-alpine
WORKDIR /app
COPY go.mod .
COPY go.sum .
RUN go mod download
COPY *.go ./
RUN go build -o /docker-go-app
EXPOSE 5003
ENTRYPOINT [ "/docker-go-app" ] 