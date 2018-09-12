# BASIC CONCEPTS

Go actually forces you to use a particular coding style.  This is a little
painful at first, but actually very good news in the long run since
it makes everyone's code look and feel the same.

Its also very fun to code.

## BASIC STRUCTURE OF GO

A go program usually has the following things,

* Package Declaration.
* Import Packages.
* Functions.
* Variables.
* Statements and Expressions.
* Comments.

## BASIC SYNTAX

`Tokens` are basically the building blocks of go.  For example,
`fmt.Println("Hello")` has six tokens.

A `Line Separator` is a statment terminator.  It's like placing a `;`.

`Comments` start with `/*` and end with `*/` or use '//'.

`Identifiers` is a name used to identify a variable, function or user defined term.

`Keywords` are reserved like `func`, `for`, `if`, `return`, etc..

`Whitespace` is ignored.

## PACKAGES

Everything in go is a package.

Here is a huge [list of go packages](http://golang.org/pkg).

Or use a go tool to look up packages,

```bash
go doc fmt
```

`import "fmt"` just imports another package.

Anything with a capital letter in a package is exported.

## RUN

```bash
go run hello.go
```

Just puts the executable in a temp location, then deletes it.

## BUILD

Compiles packages and dependencies (does not install results)
and saves your binary in current directory,

```bash
go build hello.go
./hello
```

## INSTALL

Compiles packages and dependencies and places in `/bin` and `/pkg`,

```bash
go install hello.go
$GOPATH/bin/hello
```