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

## Gate-to-Forge execution kernel

```text
Cell root and comsect1.json
-> complete immutable runtime inventory
-> language AST and binding
-> normalized proven observations
-> current Gate issues with exact AUTO_FIX candidates and direct rework IDs
-> selected AUTO_FIX: ephemeral exact plan -> apply -> same-Gate result
-> no selected mutation: initial Gate result remains current
-> current direct REWORK IDs labeled by --ai-rework on|off
```

The umbrella root has no Cell verdict. For each selected member Cell, run
`comsect1-gate check --root <cell>`. Gate and Audit remain read-only. Within
that member repository's own authority, run
`comsect1-forge fix --root <cell> --ai-rework <on|off>` when Gate identifies
the correction flow. Forge applies exact mechanical candidates without
approval, reruns the same Gate, and only labels remaining direct rework IDs; it
never launches AI. The umbrella retains only its locally shaped
`<NN>_u-<category>` groups and never acquires unit project roots.

## Author and governance

- Creator and principal architect: Kim Hyeongjeong ([@comsect1](https://github.com/comsect1))
- Architecture standard: Comsect1 Architecture
- License: Apache-2.0 with Comsect1 Template Instantiation Exception
