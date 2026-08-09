# Favo Yang Plugins

Shared Codex plugin marketplace maintained by Favo Yang.

## Install

Add this marketplace once:

```sh
codex plugin marketplace add favoyang/codex-plugins
```

Install TaskChef:

```sh
codex plugin add taskchef@favoyang-plugins
```

Start a new Codex task after installing or updating a plugin so Codex loads its
skills and tools.

## Available plugins

- [TaskChef](https://github.com/favoyang/taskchef) dispatches actionable work
  from a data-only workspace to independently openable Codex project tasks.

## Maintenance

The ordered `plugins` array in `.agents/plugins/marketplace.json` is the
catalog. Plugin source code remains in each plugin's owning repository.

Validate the catalog after changing it:

```sh
codex plugin marketplace add .
codex plugin list
```
