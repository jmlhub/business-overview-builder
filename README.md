# business-overview-builder

The human-owned standards behind the Donerail plugin's business-overview-builder skill: what an initial business overview of a public company covers, the investment principles it reads the materials through, and the research workflow. Everything here is **protected**: the skill reads it and never writes it. A change is made here by a person, or by Claude only with the user's explicit approval of a proposal showing the exact before and after, and is recorded in `specs/CHANGELOG.md`.

    business-overview-builder/
    └── specs/
        ├── business-overview.md   purpose, investment principles, research workflow, the ten sections
        └── CHANGELOG.md           every approved change, with who approved it

The memo and deck templates are not here: the plugin's document-templates skill owns the shared Donerail templates.

## How the plugin uses this repository

The plugin repository (`donerail-plugin`) vendors this repository into the skill with git subtree, so an installed plugin is self-contained:

    # first time, from the plugin repo's root
    git subtree add  --prefix=skills/business-overview-builder/standards <this repo> main --squash

    # to pull a new approved version of the standards into the plugin
    git subtree pull --prefix=skills/business-overview-builder/standards <this repo> main --squash

The skill then reads `standards/specs/`. Never edit the plugin's copy: change this repository, then pull.
