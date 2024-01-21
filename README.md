# go_basic_tutorial

Things I learned:
* Executing `go mod init {PACKAGE}/{MODULE}` creates a new Go module in the current directory
* Executing `go mod edit -replace {DEPENDENCY}={LOCAL PATH}` in a module directory will edit the Go module to use a local copy of a dependency, instead of a remote dependency
* Executing `go mod tidy` in a module directory will synchronize the module's dependencies
* Including the following code will reference a published module:

```go
require {PACKAGE}/{MODULE} {VERSION NUMBER}
```

* Executing `go run .` in a module directory with a `main` package will execute the `main` package's `main` function
* Given a module file `{MODULE}.go`, creating a file `{MODULE}_test.go` readily connects to the `go test` command
* Executing `go build` from a module directory creates an executeable `{MODULE}` on Linux and Mac, or `{MODULE}.exe` on Windows

