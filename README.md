# bug squash go

Welcome to the terrastruct go bug squash.

## setup

Please run the following to set yourself up:

```sh
cd go/src
./make.bash
PATH="$(git rev-parse --show-toplevel)/go/bin:$PATH"
```

## tests

Now you can run the tests with:

```sh
cd net/http
go test -v -timeout=30s
```

Fix the unexpected behaviour. Don't underestimate the bug, it's not a typo.

The bug is in the net/http package's code and not in the tests themselves.

This was a real bug in the python [psf/requests](https://github.com/psf/requests) library
and is often given as an interview challenge at Stripe. We modified the Go standard
library to produce the same bug.

Good luck!
