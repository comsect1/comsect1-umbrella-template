# Umbrella Classification Form and Local Authority

## Template scope

This template standardizes how an umbrella represents classification. It does
not predefine a global taxonomy, category vocabulary, repository role catalog,
or repository-prefix registry.

Every downstream umbrella owns the vocabulary, meaning, and ordering of its
categories. No category label or role is implied by this template.

## Category form

- Name every category `<NN>_u-<category>/`, where `NN` is a two-digit local
  ordering key and `<category>` is a stable lowercase kebab-case label.
- Numbers are local presentation order. They need not be contiguous and do not
  carry a universal meaning across umbrellas.
- Put each active member directly below exactly one category directory.
- A category is an ordinary umbrella-owned directory, never a repository,
  submodule, Cell, package, or implementation container.
- Give each category a boundary `README.md` that states its local inclusion and
  exclusion rules without duplicating the member list.

## Classification authority

- The downstream umbrella's governance and category boundary READMEs own its
  classification decisions.
- `.gitmodules` and committed gitlinks remain the sole membership authority.
- Preserve an existing intentional category scheme during template adoption;
  do not rename or merge categories merely to resemble another umbrella.
- Create, rename, split, merge, or retire a category only through an explicit
  umbrella-local decision that accounts for every affected member path.
- Category placement does not establish or alter member implementation
  ownership, repository role, license, Assembly identity, or Cell identity.

## Repository names and prefixes

- This template does not mandate a repository prefix or infer one from a
  category name.
- An umbrella may adopt a local naming policy, but that policy must be declared
  by the umbrella rather than presented as template or Comsect1 law.
- A repository rename is a separate identity migration. When explicitly
  authorized, update its remote, `.gitmodules` entry, local member path, and
  relevant identity documentation together.
