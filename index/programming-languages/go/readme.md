#[programming languages - go](https://my.mindnode.com/gEuiz5ncm3pdAsFYHcSe3pzbYkDxNeya7qmik71U)

![](http://i.imgur.com/QmT6FOm.png)


#mindmap index 🗄️

# terms


## unmarshalling

### parsing something

- like json


# tips


## [avoid using else](https://golang.org/doc/effective_go.html#if)

### use return, break, continue, etc

### [if else makes more sense, prefer switch / case for readability](https://golang.org/doc/effective_go.html#switch)

### avoid deep nesting of conditionals


# articles


## [getting started with go workspaces](http://gowithconfidence-blog.tumblr.com/post/118493925546/getting-started-with-go-workspaces)

### you don’t want to set GOROOT

### GOROOT tells the go command where to find the Go distribution, but unless you did a funky install, it already knows!

### Certainly if you built from source, the location of the Go distribution is compiled into the binary (though if you move it afterwards, setting GOROOT is necessary). Binary installations also know where to find things

### GOPATH, on the other hand, tells the go command where to find your source code, as well as any Go source on your machine that is not part of Go’s standard library.

- TL;DR: if you don’t want a deeper understanding of how things work, set GOPATH=$HOME/gopath, and put source in $HOME/gopath/src.

### FINISH: 

## [Monitor web page changes with Go](http://silviosimunic.com/blog/monitor-web-page-changes-with-go/)

### READ: 

## [16: the complete guide to go net/http timeouts](https://blog.cloudflare.com/the-complete-guide-to-golang-net-http-timeouts/)

### READ: 


# resources


## [go web examples](https://gowebexamples.github.io/)

### READ: 


# notes


## key is that methods can be attached to any (user-defined) type, not just structures. That includes integers, strings, even maps and arrays.

## if I plan to write any go program that I will upload to github

### I do it in my GOPATH workspace under github.com/nikitavoloboev


# go cli


## go test

### -p

- execute serially if you're testing against postgres etc across packages

	- probably better to create a random db each time 



