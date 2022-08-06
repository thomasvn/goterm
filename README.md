# Proof of Concept Terminal in Golang

Leverages the original "[freman/goterm](https://github.com/freman/goterm)" and [xterm.js](https://xtermjs.org/)

![image](https://cloud.githubusercontent.com/assets/8284169/15344054/6f3aff7a-1ce6-11e6-8e54-c2edb303f944.png)

## Running

```bash
# Clone repos
git clone https://github.com/thomasvn/goterm.git
git clone https://github.com/sourcelair/xterm.js ./assets/xterm.js

# Initialize the module. Download dependencies.
go mod init goterm
go mod tidy

# Build & run
go run main.go
```

<http://localhost:3000>

<!--
PERSONAL REFS:
- https://go.dev/doc/code
-->

<!-- 
TODO:
- Log print "received" and "sent" statements
- Document code to better understand websocket
- Dockerize (?)
- Provide warning that this is not usable
- "This is a small component of a much larger system including authentication, access control and security - do not use it."
-->

<!--
DONE:
- get it running
- understand `go get` and `go mod`
-->