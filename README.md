# PokeNexus Breeding Compatibility Chart

A fan-made breeding compatibility tool for PokeNexus (PNO), based on the game's custom breeding rules rather than standard Pokémon egg groups.

Live chart: **[diehllane.github.io/breeding](https://diehllane.github.io/breeding/)**

Note: the chart is based on the game's current rarities — any proposed rarity changes will be reflected here once they actually go live.

## Where to Breed

Visit the Pokémon breeder at the house south of Cerulean. Gender can be changed at the Gender Change NPC near the breeder for 50,000 (a genderless Pokémon cannot have its gender changed).

## Basic Compatibility

Both parents must **share at least one type** and have the **same rarity**. Rarity tiers, lowest to highest: Common, Uncommon, Rare, Very Rare, Extremely Rare, Legendary.

- **Mother slot**: a Female Pokémon, a genderless Pokémon, or Ditto
- **Father slot**: a Male Pokémon, a genderless Pokémon, or Ditto
- Shop Pokémon have a rarity already assigned to them

You cannot breed Pokémon that are untradeable, on loan, or holding an item (remove the item first).

## Genderless Pokémon

A genderless Pokémon can breed with either a male or female partner of the same rarity that shares a type. It always takes the Mother slot, so the baby is always the genderless parent's species **and form**.

Two genderless Pokémon can only breed together if they're in the same evolution line (different forms of the same species count as the same line too) — a genderless Pokémon cannot breed with a genderless Pokémon from an unrelated line.

## Ditto

Ditto ignores the type and rarity-matching rules, but only breeds with **Very Rare or lower** — it cannot pair with Extremely Rare or Legendary Pokémon. Two Ditto cannot breed together.

## Legendary Pokémon

A Legendary cannot be bred at all, unless paired with **another Pokémon of the same species that you caught yourself** (self-caught, not traded/gifted/otherwise obtained). Different forms of the same legendary still count as the same species, and the child takes the mother's form.

This exception ignores the usual gender rules — two of the same gender can breed together, and two genderless legendaries can breed together as well.

## What the Egg Inherits

Both parents are **consumed** (lost permanently) when breeding.

- The child is the baby form of the **mother's** evolution line, at level 1. If the mother slot has a Ditto, the father's line is used instead.
- Forms follow the mother (Alolan, Rotom, Oricorio, Shellos, Deerling, Vivillon, Pumpkaboo size, etc.)
- Nidoran-F bred with Nidoran-M always produces a Nidoran-M.
- No moves are passed down — the child knows only its level 1 moves.
- **IVs**: each stat is randomized within the range of the two parents (e.g. parent 1 has 5 Attack IV, parent 2 has 18 → child is randomly 5–18). An **IV Powder** locks in one parent's IV for a given stat instead of rolling the range (3 IV Powders are crafted from 1 IV Reset).
- **Nature**: random unless you spend 1 Everstone to copy one parent's nature. The Everstone doesn't need to be held — just in your inventory.
- **Ability**: random — about a 30% chance of the hidden ability, otherwise one of the normal abilities. Battle Bond is never inherited.
- **Shiny**: the child is only shiny if **both** parents are shiny.
- **Catcher name**: if either parent has your catcher name, the child counts as self-caught. Otherwise its catcher name is "Pokémon Breeder." Bred Pokémon count as seen and owned in the Pokédex, never as caught.

## Features

- Search all 807 Gen 7 Pokémon with live autocomplete
- Results grouped by shared type (or by rarity tier for Ditto, since it ignores type)
- Rarity shown on every Pokémon card
- Genderless matches (including Ultra Beasts) marked with an asterisk on other Pokémon's results, noting the egg always comes out as the genderless species
- Ditto shown at the bottom of any eligible Pokémon's results as a universal option, or searchable directly for its own full compatible list
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
