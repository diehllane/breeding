# PokeNexus Breeding Compatibility Chart — Godot Edition

A fan-made breeding compatibility tool for PokeNexus (PNO), based on the game's custom breeding rules rather than standard Pokémon egg groups.

## Breeding Rules (PokeNexus / Godot)

- Two Pokémon can breed if they **share at least one type** AND have the **same rarity**
- Rarity tiers (lowest → highest): Common, Uncommon, Rare, Very Rare, Extremely Rare, Legendary
- **Ditto** is the universal exception — it can breed with any Pokémon regardless of type or rarity
- The female parent determines which species the egg will be

## Features

- Search all 807 Gen 7 Pokémon with live autocomplete
- Results grouped by shared type
- Rarity shown on every Pokémon card
- Ditto always shown at the bottom as a universal option
- Live type data from PokéAPI; rarity data sourced from the PokeNexus game guide

## Deployment (GitHub Pages)

1. Create a new GitHub repository
2. Upload `index.html` to the repo root
3. Settings → Pages → Source: `main` branch, `/ (root)`
4. Live at `https://<username>.github.io/<repo-name>/`

Only one file needed — no images, no build step.

## Data Sources

- Types: [PokéAPI](https://pokeapi.co)
- Sprites: [PokeAPI Sprites](https://github.com/PokeAPI/sprites)
- Rarity: PokeNexus official game guide
