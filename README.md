# GoContainerHello
 Sample container rest api in Go using Gin

### Run
```
go get -u github.com/gin-gonic/gin
go run main.go
```
- Make a get request to http://localhost:8080/ping will get a response of "pong"
- Or run that in the tests.http (Using VS Code Rest Client extension)

### Build Container
```
docker build . -t gocontainerapi:latest
```

### Run Container
```
docker run -e PORT=9000 -p 9000:9000 gocontainerapi:latest
```
- Make a get request to http://localhost:9000/ping will get a response of "pong"
- Or run that in the tests.http

### Refences:
- Great video: https://www.youtube.com/watch?v=C5y-14YFs_8