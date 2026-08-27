# Comsect1 Umbrella Template Licensing Policy

This repository is the upstream licensing-policy SSOT for umbrella templates.
The root [LICENSE.md](../LICENSE.md) controls the template's own material.

## Independent authorities

- The umbrella scaffold, instructions, category READMEs, and root governance
  files use Apache-2.0 with the Comsect1 Template Instantiation Exception.
- Every member gitlink refers to an independent repository with its own owner,
  history, license, notices, dependencies, and release policy.
- Category placement, `.gitmodules`, an umbrella license, or an aggregate build
  never relicenses a member.
- Retained third-party and downstream material keeps its original terms.

## Membership and distribution checks

1. Verify each member exposes an unambiguous license and required notices.
2. Record the exact member commit; review the license at that commit.
3. Evaluate compatibility for the actual aggregate distribution, linking, and
   deployment model. Mere coexistence as gitlinks is not license combination.
4. Preserve member notices and produce an aggregate notice or SBOM only when a
   distribution actually includes member material.
5. Do not copy member source or license-controlled artifacts into the umbrella.

The template instantiation exception permits an independent downstream
umbrella. It does not transfer ownership of members or waive their licenses.
