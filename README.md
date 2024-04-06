# ccproducers

Fork from dinowernli/ccproducers. Various bug fixes and code cleanup.

A producer graph implementation in c++. For details on producers, see http://google.github.io/dagger/producers.html.

## Building and running

In order to build and run tests, execute

`> bazel test ...`


## How

In WORKSPACE add
```WORKSPACE
http_archive(
  name = "ccproducers", 
  sha256 = "5b9f37f55cd48cc714bdd410164c1f37a8a0df588d11373091503a081765e360",
  strip_prefix = "ccproducers-0.0.2",
  urls = ["https://github.com/chokychou/ccproducers/archive/refs/tags/v0.0.2.tar.gz"],
)

```

In BUILD add
`"@ccproducers//:producer_graph",
`
