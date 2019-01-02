# Go

Golang is an open source programming language maintained by Google. 

## Installation

Go can be installed by brew as:

```
$ brew install go
```

You can run `go version` to verify installation and to check version.

## Setup workspace

Go has a unique approach of managing workspace for all your Golang projects, dependencies, packages etc. Firstly, you will have to set environment variables for this workspace. `GOROOT` is the location of Go installation. This should be added to PATH variable which looks like:

```
export GOROOT= /usr/local/Cellar/go/1.4.2/libexec
export PATH=$PATH:$GOROOT
```
You can also add this environment to shell config file like `.zshrc`, `.bashrc`.

Consider `$HOME/go` to be your Go project workspace. To setup your workspace, you will need to create three directories within it as follows.

```
mkdir -p $GOPATH $GOPATH/src $GOPATH/pkg $GOPATH/bin
```
`GOPATH` variable should be set to location of Go project workspace. Within this workspace, the src directory holds all the source code, pkg holds the compiled bits, and bin directory holds all the executables. As bin holds all the executables, this should be added to PATH as well.

```
export GOPATH=$HOME/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:$GOPATH/bin
```

## Test installation

A simple go program can be written and tested to check the correctness of our installation.

A file named `test.go` can be created in `$GOPATH/src` with program written as:
```
package main

import "fmt"

func main(){
	fmt.Printf("Testing go installation. It works!!\n")
}
```
Run program by:

```
$ go run test.go
Testing go installation. It works!!
```

If the message is printed as shown, then the Go installation is working properly. 

This creates a binary called `test` in `GOBIN` which is also added to `PATH` variable. So you can run `test` from anywhere to run this program.


