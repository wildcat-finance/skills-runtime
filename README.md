# Wildcat skills runtime

Every file here is generated. Nothing in this repository is authored, and an
edit made here is overwritten by the next rebuild.

The source is [wildcat-finance/skills](https://github.com/wildcat-finance/skills).
This package was generated from commit `a2b634d8e039af988bf30c8316defccf70071d8d` by
`scripts/portable_promise_machine.py` in that repository.

## Install

```
npx skills add wildcat-finance/skills-runtime --skill promise-machine
```

Then verify the installed copy against its own manifest:

```
python3 .agents/skills/promise-machine/scripts/verify_runtime.py
```

## Rebuilding

A scheduled workflow in this repository clones the public source hourly,
regenerates the package, verifies it, and commits only when the bytes changed.
A failed verification publishes nothing and fails the run, so the last good
package stays published.

Changes belong upstream. Open issues and pull requests against
`wildcat-finance/skills`.
