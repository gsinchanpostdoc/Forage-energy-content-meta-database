# 🌿 Forage Energy Database

A community-maintained web application for computing and comparing the **preference-weighted metabolizable energy (e_p)** of plant forage species for ungulates.

**Live app:** [https://gsinchanpostdoc.github.io/Forage-energy-content-meta-database/](https://gsinchanpostdoc.github.io/Forage-energy-content-meta-database/)

**Google Site:** [Energy Content in Forage](https://sites.google.com/view/sinchan-ghosh/metadatabases/energy-content-in-forage)

## The Model

```
e_p = ME × Preference Index
```

Where:
- **ME** (Metabolizable Energy) = 15.2×CP + 15.9×NSC + 34.2×Lipids + 12.8×dNDF
- **dNDF** = Fibre × (% digestible NDF) / 100
- **Preference Index** = Ranked Jacobs D selectivity index
- Energy coefficients from **Menke et al.**
- Selectivity index from **Jacobs (1974)**

## Features

| Feature | Description |
|---------|-------------|
| **Database Browser** | Sortable, filterable table of all forage energy records. Pre-loaded with 24 moose records (6 plants × 4 seasons). |
| **ME Calculator** | Enter plant chemistry values to compute metabolizable energy and e_p interactively. |
| **Contribute Data** | Two pathways: (A) email a data request, or (B) enter data directly into the shared database. |
| **Community Database** | User-contributed records persist in browser storage and are visible to all visitors. |

## Pre-loaded Data

The database ships with moose (*Alces alces*) data for 6 plant categories across 4 seasons:

- **Plants:** Broadleaf, Common juniper, Pine, Shrub, Spruce, Bilberry
- **Seasons:** Spring, Summer, Autumn, Winter
- **Values:** Plant chemistry (CP, NSC, Lipids, Fibre, dNDF%), Jacobs D, Preference Index, ME, e_p

## Deployment

This is a **zero-build, single-file application**. No Node.js, npm, or build step required.

The `index.html` file contains the entire app. Simply enable GitHub Pages (Settings → Pages → main branch / root) and it is live.

It is also embedded in the Google Site at [Metadatabases → Energy Content in Forage](https://sites.google.com/view/sinchan-ghosh/metadatabases/energy-content-in-forage).

## Variables

| Variable | Description | Unit |
|----------|-------------|------|
| CP | Crude Protein — digestible fraction (Menke et al.) | g/100g DM |
| NSC | Non-Structural Carbohydrate — digestible fraction | g/100g DM |
| Lipids | Lipids — digestible fraction | g/100g DM |
| Fibre | Total fibre content | g/100g DM |
| dNDF% | Percentage of NDF that is digestible | % |
| dNDF | Digestible Neutral Detergent Fibre | g/100g DM |
| ME | Metabolizable Energy | MJ/kg DM |
| Jacobs D | Selectivity index (-1 to +1) | — |
| Pref. Index | Ranked Jacobs D | — |
| e_p | Preference-weighted energy content | MJ/kg DM |

## Key References

- Menke et al. — Energy coefficients for ruminant metabolizable energy
- Jacobs, J. (1974) — Quantitative measurement of food selection
- Shipley, L.A. (1998, 1999) — Moose digestibility and foraging parameters
- Dungan, J.D. (2010) — Moose energy expenditure and harvesting rates
- Wam, H.K. (2010) — Seasonal moose diet composition
- Renecker, L.A. & Hudson, R.J. (1992) — Moose basal metabolic rate

## Links

- [Energy Content in Forage (Google Site)](https://sites.google.com/view/sinchan-ghosh/metadatabases/energy-content-in-forage)
- [Sinchan Ghosh — Main Site](https://sites.google.com/view/sinchan-ghosh)

## Contact

Maintained by **Sinchan Ghosh** — sinchanghosh110@gmail.com

## License

MIT
