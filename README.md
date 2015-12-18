# force

force is a Go client library for accessing the [Salesforce API][].

**Documentation:** [![GoDoc](https://godoc.org/github.com/jpmonette/force?status.svg)](https://godoc.org/github.com/jpmonette/force)  

## Usage

```go
import "github.com/jpmonette/force"
```

### Authentication

The force library does not directly handle authentication.  Instead, when
creating a new client, pass an `http.Client` that can handle authentication for
you.  The easiest and recommended way to do this is using the [oauth2][]
library, but you can always use any other library that provides an
`http.Client`.


## Roadmap

This library is being initially developed for one of my internal project,
so API methods will likely be implemented in the order that they are
needed by my project. Eventually, I would like to cover the entire
Salesforce API, so contributions are of course [always welcome][contributing].  The
calling pattern is pretty well established, so adding new methods is relatively
straightforward.

[contributing]: CONTRIBUTING.md


## License

This library is distributed under the MIT license found in the [LICENSE](./LICENSE)
file.