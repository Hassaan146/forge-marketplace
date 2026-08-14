# Forge Marketplace

The install source for **[Forge Mentor](https://github.com/Hassaan146/forge-mentor)** —
a Claude Code plugin that teaches every load-bearing decision, records your choice, and
blocks code from moving past a decision you have not made yet.

## Install

```
/plugin marketplace add Hassaan146/forge-marketplace
/plugin install forge@forge-marketplace
```

Forge requires ponytail, which is in this same marketplace, so it is one more command and
no second marketplace to add:

```
/plugin install ponytail@forge-marketplace
```

Then, once per project:

```
/forge:start
```

Restart Claude Code after installing either one. Hooks and the engine are registered at
startup, so a plugin installed mid-session loads nothing until you quit and reopen.

## Plugins here

| Plugin | What it does |
|---|---|
| `forge` | Forge Mentor — decide-then-code mentoring pipeline |
| `ponytail` | Keeps the generated code small: does this need writing, does the project already do it, does the standard library do it. By [Dietrich Gebert](https://github.com/DietrichGebert), MIT. Forge routes to it at the building and review steps and will not finish setup without it. |

## License

MIT
