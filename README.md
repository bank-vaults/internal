# Bank-Vaults internal libraries

[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/bank-vaults/internal/ci.yaml?branch=main&style=flat-square)](https://github.com/bank-vaults/internal/actions/workflows/ci.yaml?query=workflow%3ACI)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/bank-vaults/vault-env/badge?style=flat-square)](https://api.securityscorecards.dev/projects/github.com/bank-vaults/internal)

**Internal libraries used by Bank-Vaults components.**

## Development

**For an optimal developer experience, it is recommended to install [Nix](https://nixos.org/download.html) and [direnv](https://direnv.net/docs/installation.html).**

_Alternatively, install [Go](https://go.dev/dl/) on your computer then run `make deps` to install the rest of the dependencies._

Make sure Docker is installed with Compose.

Fetch required tools:

```shell
make deps
```

Run project dependencies:

```shell
make up
```

Run the test suite:

```shell
make test
```

Run linters:

```shell
make lint # pass -j option to run them in parallel
```

Some linter violations can automatically be fixed:

```shell
make fmt
```

Once you are done, you can tear down project dependencies:

```shell
make down
```

## License

The project is licensed under the [Apache 2.0 License](LICENSE).
