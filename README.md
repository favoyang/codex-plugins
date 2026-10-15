# Favo Yang Plugins

Shared Codex plugin marketplace maintained by Favo Yang. The catalog currently
contains no plugins.

## TaskChef has moved

TaskChef now owns its marketplace in the [TaskChef repository](https://github.com/favoyang/taskchef).
Add its marketplace and install the released plugin:

```sh
codex plugin marketplace add favoyang/taskchef
codex plugin add taskchef@taskchef
```

After the new installation succeeds, remove `taskchef@favoyang-plugins` and
restart Codex. Keep only one released TaskChef installation enabled. TaskChef
Dev uses a separate local marketplace and can stay enabled. Settings, GitHub
credentials, and Codex chat history do not need to be reset.

```sh
codex plugin remove taskchef@favoyang-plugins
```

## Maintenance

The ordered `plugins` array in `.agents/plugins/marketplace.json` is the catalog.
Each plugin's source code and release workflow belong to its owning repository.
TaskChef's release workflow no longer updates this catalog.
