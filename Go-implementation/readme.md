## Getting started with in_toto golang version

Go implementation of in-toto is based on in-toto Python reference implementation. Below are the steps to setup this implementation in your local machine and test it.

1.	Install Go tools(version 1.11) in your local machine. Follow the installation method from this link -> https://golang.org/doc/install

Here is a quick video on go. This video is a great staring point in understanding basic go concepts https://www.youtube.com/watch?v=C8LgvuEBraI&t=724s

2.	Once installed successfully, you should be able to use 'go' as a command on your terminal just like 'git'.
3.	Now clone in-toto-golang repository in your local machine by running below command:
			```
			git clone https://github.com/in-toto/in-toto-golang.git 
			```
4.	Now run the command on your terminal:  
			```
			godoc -http :8080
			```
	and then navigate to localhost:8080/pkg/github.com/in-toto/in-toto-golang/in_toto/ to read about the documentation of go-lang implementation of in-toto.

	Here is the link for in_Toto documentation.
	https://github.com/in-toto/docs/blob/master/in-toto-spec.md

5.	Entire codebase of this implementation is in in-toto folder of the repo.
6.	After making any changes to the repo you can run below command from root project directory to test whether your changes are working correctly with other functionalities or breaking the code.
			```
			go test ./...
			```
or you can run ```
			go test
			```
			from the in_toto directory.