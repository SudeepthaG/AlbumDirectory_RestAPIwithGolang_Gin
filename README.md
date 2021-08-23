# AlbumDirectory_RestAPIwithGolang_Gin

This repository implements an album directory which can be used to add an album to a directory and get details of all albums/a specific album.

I have used Golang and Gin framework for this purpose.

## Steps to implement

- Clone this repository
- cd to this folder
- In terminal type: go get -u github.com/gin-gonic/gin
- go mod init example.com/AlbumDirectory_RestAPIwithGolang_Gin

### To get details about all albums use:

- go get .
- go run .
- From a new command line window, use curl to make a request to your running web service. $curl http://localhost:8080/albums

### To get details about a specific album use:

- go get .
- go run .
- $ curl http://localhost:8080/albums/2 Here 2 is your album number

### To add an album use:

- go get .
- go run .
- $ curl http://localhost:8080/albums \

  --include \

  --header "Content-Type: application/json" \

  --request "POST" \

  --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
