# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **GitHub profile README** repository. Its only tracked file is
`ReadMe.md`, which GitHub renders on a profile page.

There is **no application, no test suite, no lint config, and no build system**, and there
are no dependency manifests (no `package.json`, `requirements.txt`, etc.). As a result:

- There is nothing to install for normal development. The startup update script is a no-op.
- There is no lint / test / build / run command for a product.
- "Developing" here means editing `ReadMe.md` (GitHub-Flavored Markdown).

### Previewing the README (optional)

To preview the README the way GitHub renders it, you can use `grip` (not a project
dependency; install ad hoc if needed):

```
pip install --user grip
~/.local/bin/grip ReadMe.md 0.0.0.0:6419
```

`grip` uses GitHub's rendering API, so it needs outbound network access.
