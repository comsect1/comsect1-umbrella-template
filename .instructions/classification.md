# Comsect1 Architecture Classification and Repository Taxonomy SSOT

This document defines the normative Single Source of Truth (SSOT) for umbrella
categorization (`<NN>_u-<category>/`), member repository classification, and standardized
repository prefix naming conventions across the Comsect1 architecture ecosystem.

---

## 1. Core Principles

1. **Durable Responsibility**:
   - Each active member belongs directly below exactly one stable numbered
     `<NN>_u-<category>/` directory.
   - Categories express durable architectural responsibility, not current team
     ownership, transient technology, release state, or temporary initiatives.
2. **Deterministic Prefix Alignment (3-Letter Hierarchy)**:
   - Member repositories MUST follow the standardized `[domain]-[type]-[name]`
     hierarchical naming format.
   - This ensures lexicographical ordering, automated CI/CD filtering, and clear
     role boundaries across polyrepo workspaces.
3. **SSOT Lineage & Downstream Inheritance**:
   - This taxonomy is canonically defined in `comsect1`.
   - Downstream enterprise templates (e.g., `hatbit-*-template`) inherit this SSOT
     to enforce uniform governance across proprietary repositories.

---

## 2. Standard Repository Prefix and Numbered Category Taxonomy

### A. Component Domain (`*-components`)

| Numbered Category Directory | Standard Prefix | Meaning & Scope | Examples |
| :--- | :---: | :--- | :--- |
| `10_u-drivers/` | **`cmp-drv-*`** | Hardware peripheral / MCU abstraction driver | `cmp-drv-ind83213`, `cmp-drv-efr32-bg22` |
| `20_u-libraries/` | **`cmp-lib-*`** | Reusable protocol, math, or utility library | `cmp-lib-com`, `cmp-lib-os`, `cmp-lib-std` |
| `30_u-runtimes/` | **`cmp-rt-*`** | Core execution runtime / HAL engine | `cmp-rt-physical`, `cmp-rt-graphics` |
| `40_u-plugins/` | **`cmp-plg-*`** | Extensible tool / editor plugin | `cmp-plg-ai-adapters`, `cmp-plg-linter` |
| `50_u-assemblies/` | **`cmp-asm-*`** | Multi-component integrated composite | `cmp-asm-ambientlight`, `cmp-asm-heater` |

---

### B. Product Domain (`*-products`)

| Numbered Category Directory | Standard Prefix | Meaning & Scope | Examples |
| :--- | :---: | :--- | :--- |
| `10_u-foundations/` | **`prd-fnd-*`** | Domain foundation, core doctrine, or persona theory | `prd-fnd-polaris`, `prd-fnd-quadrant` |
| `20_u-platforms/` | **`prd-plt-*`** | Core infrastructure, backend, or communication platform | `prd-plt-artifact-platform`, `prd-plt-data-comm-bridge` |
| `30_u-tools/` | **`prd-tool-*`** | Engineering, developer, or automation tooling | `prd-tool-autosar-classic-ide`, `prd-tool-ruleforge` |
| `40_u-apps/` | **`prd-app-*`** | Standalone executable application (desktop/mobile/CLI) | `prd-app-lin-remaster`, `prd-app-sl-moodlamp-studio` |

---

### C. Auxiliary Domains

| Domain Umbrella | Numbered Category Directory | Standard Prefix | Meaning & Scope | Examples |
| :--- | :--- | :---: | :--- | :--- |
| `*-labs` | `10_u-trials/` | **`lab-*`** | Proof-of-concept (PoC), laboratory trials, and research studies | `lab-spacedevkit-satellite`, `lab-mppt-arduino-uno` |
| `*-presentation` | `10_u-presentations/` | **`prs-*`** | Technical presentations, slide decks, and architecture models | `prs-software-development` |
| `*-archived` | `99_u-archives/` | **`arc-*`** | Decommissioned or preserved historical assets | `arc-holonyak`, `arc-lin-commander-pic16f` |

---

## 3. Governance and Invariance Rules

- **Category Isolation**: A category `README.md` defines purpose and boundary exclusions without duplicating the member list governed by `.gitmodules`.
- **Identity Invariance**: Category paths within an umbrella do not alter the fundamental Cell/Assembly identity of the member repository.
- **Prefix Consistency**: Renaming a repository to conform with this taxonomy must update both the remote repository name, the local `.gitmodules` submodule path, and the root `README.md`.
