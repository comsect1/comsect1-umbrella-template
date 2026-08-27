# Comsect1 Umbrella Template

Fork this repository to classify and pin independent repositories without
absorbing their implementation, Git history, Cell authority, or licenses.

The umbrella owns only numbered member categories and their Git membership
index. During adoption, create the `<NN>_u-<category>/` directories needed by
the umbrella and register members through `.gitmodules`. Project roots such as
`10_pkg/`, `20_ops/`, and `30_cert/` belong to unit repositories, not umbrellas.

The scaffold itself is the Comsect1 upstream SSOT. Downstream enterprise forks
must preserve its structural meaning and record their ownership and licensing
transformation without rewriting member licenses.

See [AGENTS.md](./AGENTS.md) and the [instruction index](./.instructions/README.md).

## Author and governance

- Creator and principal architect: Kim Hyeongjeong ([@comsect1](https://github.com/comsect1))
- Architecture standard: Comsect1 Architecture
- License: Apache-2.0 with Comsect1 Template Instantiation Exception
