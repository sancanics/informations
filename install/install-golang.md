# Install Go Programming Language

1. Download go from the official website: [Golang](https://go.dev/dl/).
2. Choose the latest version of go.
3. Delete old go version if you have been installed go already
```bash
$ sudo rm -rf /usr/local/go
```
4. Untar go package:
```bash
$ ~ cd downloads
$ [downloads] tar -xzf go1.20.3.linux-amd64.tar.gz
```
5. move go folder into this directories:
```bash
$ [downloads] sudo mv go /usr/share/local/go
```
6. add the following into `.profile` or `.bash_profile`:
```bash
export GOPATH="$XDG_DATA_HOME/go"
export GOROOT="/usr/local/share/go"
export GOMODCACHE="$XDG_CACHE_HOME/go/mod"
export PATH="$GOROOT/bin:$GOPATH/bin:$PATH"
```
7. source the `.profile` or `.bash_profile` or if you want, **logout** and then **login** to activate our go configuration.
8. check go if installed correctly:
```bash
$ go version
```

**NOTES:**

- `$XDG_DATA_HOME` and `$XDG_CACHE_HOME` is just XDG base dir specifications.
- code that we add into `.profile` or `.bash_profile` is from [archlinux base dir](https://wiki.archlinux.org/title/XDG_Base_Directory)
- Golang official docs : [links](https://go.dev/doc/install)

its just xdg base dir specification: [Read More](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
