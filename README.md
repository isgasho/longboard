# Longboard: The easy way to [surf](https://github.com/http-rs/surf)

```bash
$ longboard get https://async.rs
```


## TODO for this to be useful
- [x] request bodies
  - [x] from filesystem
  - [x] as a cli arg
  - [x] from stdin (pipe)
- [x] request headers
- [ ] opt into / out of displaying different parts of request and response
- [ ] http status -> exit codepp



<!-- * [CI ![CI][ci-badge]][ci] -->
* [Releases][releases] [![crates.io version][version-badge]][lib-rs]
* [Contributing][contributing]

<!-- [ci]: https://github.com/jbr/longboard/actions?query=workflow%3ACI -->
<!-- [ci-badge]: https://github.com/jbr/longboard/workflows/CI/badge.svg -->
[releases]: https://github.com/jbr/longboard/releases
[contributing]: https://github.com/jbr/longboard/blob/master/.github/CONTRIBUTING.md
[lib-rs]: https://lib.rs/longboard
[version-badge]: https://img.shields.io/crates/v/longboard.svg?style=flat-square

## Installation

```sh
$ cargo install longboard --version 0.0.2-alpha.3
```

## Usage

```sh
longboard 0.0.2-alpha.3
the easy way to surf

USAGE:
    longboard [OPTIONS] <method> <url>

FLAGS:
        --help       Prints help information
    -V, --version    Prints version information

OPTIONS:
    -b, --body <body>             provide a request body on the command line
    -c, --client <client>         http backend for surf. options: h1, curl, hyper [default: h1]
    -f, --file <file>             provide a the path to a file to use as the request body
    -h, --headers <headers>...    provide headers in the form -h KEY1=VALUE1 KEY2=VALUE2

ARGS:
    <method>
    <url>
```

## Safety
This crate uses ``#![forbid(unsafe_code)]`` to ensure everything is implemented in
100% Safe Rust.

## License

<sup>
Licensed under either of <a href="LICENSE-APACHE">Apache License, Version
2.0</a> or <a href="LICENSE-MIT">MIT license</a> at your option.
</sup>

<br/>

<sub>
Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in this crate by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.
</sub>
