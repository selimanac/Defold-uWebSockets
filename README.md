# Defold uWebsockets

_**Caution!** Not developing anymore._

This project is build by using [uWebsockets 0.14](https://github.com/uNetworking/uWebSockets/tree/v0.14) and its dependencies. 

Currently testing on MacOS 10.14.3, iOS 9.3.5

### Known issues  

- MacOS and iOS only. Windows, Linux and Android not supported yet. Libraries need to build for those platforms.
- Using SSL (wss) cause crash. OpenSSL cause this.
- Not tested with 64 bit iOS devices yet.

------

### API


#### uwebsockets.connect  
uwebsockets.connect(host, name, callback, time out)

`host` "ws://" .. server_adress .. ":" .. server_port .. "/" .. room_name  
`name` connection name  
`callback` lua callback   
`time out` connection time out

#### uwebsockets.send   
uwebsockets.send(name, string)

`name` connection name  
`string` string like json 

#### uwebsockets.close
uwebsockets.send(name)  
`name` connection name  
