# Umbrella Temporary Output and Cleanup

An umbrella has no local temporary-output or trash root. Put every Gate, Forge,
integration, generation, and verification run in an explicitly supplied
directory outside the umbrella and every member repository.

Never place generated inventory, evidence, progress logs, caches, or staging
inside a category or member. Cleanup is governed by the external workspace that
owns the run directory; umbrella authority does not authorize deleting any
member path, category, repository root, or unknown external output.
