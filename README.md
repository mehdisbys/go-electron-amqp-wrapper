go-electron-amqp-wrapper
===========================

A wrapper for the AMQP v1.0 electron library using ActiveMQ


![ActiveMQ](https://upload.wikimedia.org/wikipedia/commons/4/42/Apache-activemq-logo.png)

This is a basic POC for creating AMQ Producer and Consumer with Go:




Pre-Requisites:

 - Install Go and ActiveMQ on Mac : ``` brew install go ActiveMQ```
 - Add these lines to your bashrc :
 ```
 export PATH=$PATH:/usr/local/opt/go/libexec/bin
 export GOPATH=/usr/local/opt/go/bin
```
- Start ActiveMQ : ```activemq start```
- Check everything is working well by logging into the web ActiveMQ console : [http://localhost:8161/admin/](http://localhost:8161/admin/)
- Console passd/username are : admin/admin


Install:

- From inside the cloned repository

```
go get
```

Run Producer:
```
go run sender.go
```

Run Consumer:
```
go run reader.go
```

### Experiment

Run 10000 msg and time how long it took for producer and consumer

