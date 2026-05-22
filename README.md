# ForgeTools

A collection of web-based tools for **Supreme Commander: Forged Alliance Forever (FAF)** — hosted at [seraphimnoob01.github.io/ForgeTools](https://timmasalme.github.io/ForgeTools/).

---

## Tools

### Shield Assist Calculator
Calculate how many engineers you need to keep a T3 shield alive under T3 or experimental artillery fire.

- Supports all T3 artillery (Duke, Disruptor, Emissary, Hovatham) and experimentals (Mavor, Salvation)
- Supports all T3 shields (HSD Pulse, ED4, ED5, Radiance, Athanuhthe)
- Accounts for T3 Power Generator adjacency / reload bonuses
- Live data fetched from [etfreeman-db](https://faforever.github.io/etfreeman-db/) and the [FAForever/fa](https://github.com/FAForever/fa) blueprint repository

---

## Data Sources

| Source | Used for |
|---|---|
| [etfreeman-db](https://faforever.github.io/etfreeman-db/data/index.json) | Shield HP, regen rate, build cost — game-accurate simulated values |
| [FAForever/fa](https://github.com/FAForever/fa) `unit.bp` | `RegenAssistMult` per shield, arty weapon stats (fallback) |
| Hardcoded constants | UEF shield `RegenAssistMult` (not present in blueprint) |

All values are fetched live on page load and fall back gracefully if a source is unreachable.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT — see [LICENSE](LICENSE).
