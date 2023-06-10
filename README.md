# Toolkit Project

Project built following Udemy course: https://www.udemy.com/course/building-a-module-in-go-golang/learn/lecture/32950244#overview

# Toolkit

A simple example of how to create a reusable Go module with commonly used tools.

The included tools are:

- [ ] Read JSON
- [ ] Write JSON
- [ ] Produce a JSON encoded error response
- [X] Upload a file to a specified directory
- [ ] Download a static file
- [X] Get a random string of length n
- [ ] Post JSON to a remote service
- [ ] Create a directory, including all parent directories, if it does not already exist
- [ ] Create a URL safe slug from a string

## Installation

`go get -u github.com/mealies/toolkit`

## Toolkit folder

This is the go module we are building, containing our tools and test files.

Not included is the app folder in the same go workspace used to test the package.

## Calling methods in this package

From your main package, you can call the packages such as the RandomSrting package like so:

```
var tools toolkit.Tools

fmt.Println(tools.RandomString(25))
```
	
	
## Go Workspace

[Go Workspaces Tutorial](https://go.dev/doc/tutorial/workspaces)

cmd `go work init toolkit app` used to create a go workspace containing these two folders.
this is go 1.18 and above