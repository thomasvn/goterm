# Proof of Concept Terminal in Golang

Leverages the original "[freman/goterm](https://github.com/freman/goterm)" and [xterm.js](https://xtermjs.org/)

![image](https://cloud.githubusercontent.com/assets/8284169/15344054/6f3aff7a-1ce6-11e6-8e54-c2edb303f944.png)

This is a completely insecure daemon that permits anyone to connect and control your computer, please don't run this anywhere.

## Running

```bash
# Clone repo
git clone https://github.com/thomasvn/goterm.git

# Initialize the module. Download dependencies.
go mod init goterm
go mod tidy

# Build & run
go run main.go
```

<http://localhost:3000>

## Architecture

The HTTP Server and Websocket Handler are written in Go.
The static frontend files import `xterm.js`, and create a new terminal for every websocket connection to the server.

<!--
PERSONAL REFS:
- https://go.dev/doc/code
- https://go.dev/doc/comment
-->

<!-- 
TODO:
- Document code to better understand websocket
- Log print "received" and "sent" statements
- Dockerize (?)
-->

<!--
DONE: (most recent to least recent)
- Why does "/term" have to come before "/"?
- Provide warning that this is not usable
- Get it running
- Understand `go get` and `go mod`
-->