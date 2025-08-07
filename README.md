# errgroup

This repository is a light fork of the `errgroup` package found in
[golang.org/x/sync](https://golang.org/x/sync). We created a new module so we
could stop adding `replace` directives as other dependencies required different
`x/sync` versions.

The primary difference between this package and upstream is the ability to determine if the `errgroup` has reported an error before `Wait()` returns.
