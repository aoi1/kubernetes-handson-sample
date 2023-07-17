# kubernetes-handson-sample

## About docker directory

The main.go is a simple HTTP server.

To run the program, all you need to do is

```
go run main.go
```


You can build docker container using:

```
cd docker/
docker build .
```

And also, you can access to the main program using:

```
docker run -p 8080:8080
```
