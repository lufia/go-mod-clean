# go mod testrepo

```console
$ git clone https://github.com/lufia/go-mod-clean
$ cd go-mod-clean
$ export GO111MODULE=off
$ go clean && echo ok
ok
$ export GO111MODULE=on
$ go clean && echo ok
can't load package: package github.com/lufia/go-mod-clean: unknown import path "github.com/lufia/go-mod-clean": cannot find module providing package github.com/lufia/go-mod-clean
$ go clean ./... && echo ok
ok
```
