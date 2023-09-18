# Golang Graphql

> Playing with Graphql

1. [Requirements](#requirements)
2. [Setup](#setup)

## Requirements

1. Go 1.20+ installed
2. Text editor such as [vs code](https://code.visualstudio.com/) or sublime text
3. Git - preferrably use terminal like [gitbash](https://gitforwindows.org/)

## Setup

1.  Mod init your project

```
    go mod init github.com/robinmuhia/GoGraphql
```

2.  Get gql gen for this project

```
    go get github.com/99designs/gqlgen
```

3.  On windows, add gqlgen to tools.go

```
    echo // +build tools^
    package tools^
    import \_ "github.com/99designs/gqlgen" > tools.go
```

4.  Initialize your project

```
    go run github.com/99designs/gqlgen init
```

5.  Get all the dependencies

```
    go mod tidy
```

6.  After you've written the graphql schema, run this

```
    go run github.com/99designs/gqlgen generate
```
