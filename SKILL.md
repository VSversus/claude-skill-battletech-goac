---
name: battletech-gac
description: >
  Kompletní znalostní základna pravidel BattleTech: A Game of Armored Combat (GoAC).
  Použij tento skill vždy, když uživatel klade otázky o pravidlech BattleTech, řeší spornou
  situaci při hře, potřebuje rychlou referenci tabulek, chce pochopit herní mechaniky,
  učí nové hráče, nebo tvoří scénáře. Triggery: "battletech", "BattleMech", "'Mech",
  "GoAC", "pravidla BT", "jak funguje [cokoliv herního]", "je to správně?", "ověř pravidlo",
  "explain battletech", "scénář", "tvorba mechů". Platí i pro fragmenty dotazů jako
  "heat", "PSR", "to-hit", "cluster hits", "critical hit", "fyzický útok", "iniciativa" apod.
---

# BattleTech: A Game of Armored Combat — Skill

Tento skill pokrývá **kompletní pravidla GoAC** (introductory ruleset). Při zodpovídání
otázek vždy odkazuj na konkrétní reference soubory, kde jsou detaily.

## Obsah reference souborů

Před odpovědí načti relevantní soubor(y):

| Soubor | Obsah |
|--------|-------|
| `references/core-sequence.md` | Sekvence hry, fáze, setup, iniciativa, vítězné podmínky |
| `references/movement.md` | Pohyb, typy pohybu, terén, skoky, prone, voda |
| `references/combat.md` | LOS, palebné oblouky, to-hit, GATOR, modifikátory, speciální útoky |
| `references/physical-attacks.md` | Fyzické útoky (charge, kick, punch, DFA, club, push) |
| `references/damage.md` | Poškození, critical hits, efekty, destrukce lokací, přenos poškození |
| `references/heat.md` | Heat management, efekty přehřátí, shutdown |
| `references/other-actions.md` | PSR (Piloting Skill Rolls), pád, displacement, poškození pilota |
| `references/tables.md` | **VŠECHNY tabulky** — to-hit modifikátory, hit location, cluster hits, PSR tabulky atd. |
| `references/weapons-equipment.md` | Zbraně a vybavení, jejich statistiky a speciální pravidla |
| `references/construction.md` | Stavba mechů (8 kroků), tonnage, engine, armor, sloty |
| `references/scenarios.md` | Hotové scénáře, tvorba scénářů, planetary conditions, kampaně |
| `references/rulebook-full.md` | **KOMPLETNÍ TEXT RULEBOOOKU se stránkami** — primární autoritativní zdroj, 1555 řádků |

## Jak pracovat s tímto skillem

**Rychlá reference při hře:** Načti `tables.md` pro okamžitý přehled čísel.

**Sporná situace:** Načti příslušný reference soubor a cituj konkrétní pravidlo.

**Výuka nových hráčů:** Začni s `core-sequence.md`, pak `movement.md`, pak `combat.md`.

**Tvorba scénářů:** Viz `scenarios.md` a `construction.md`.

## Primární zdroj — Kompletní Rulebook

Pokud odpověď není jednoznačně pokryta v reference souborech, **načti přímo**:

**`references/rulebook-full.md`** — kompletní přepis ruleboouku *BattleTech: A Game of Armored Combat* (Catalyst Game Labs, 2018) se všemi stránkami ve formátu `(str. X)`. Jedná se o tentýž zdroj, ze kterého byly sestaveny všechny ostatní reference soubory.

Protože soubor má 1555 řádků, pro efektivní vyhledávání:
- Hledej podle nadpisu sekce (např. `## HEAT`, `## COMBAT`, `### PHYSICAL ATTACKS`)
- Stránky jsou značeny inline jako `(str. X)` nebo `## NÁZEV SEKCE (str. X)`
- Načti jen relevantní část, ne celý soubor

Po nalezení odpovědi z ruleboouku:
1. Odpověz na otázku
2. Přidej citaci s přesnou stránkou a odstavcem
3. Zvaž, zda informaci doplnit do příslušného reference souboru

## Povinný formát odpovědi — citace

Ke **každé odpovědi na pravidlovou otázku** vždy přidej na konec citaci ve formátu:

> 📖 *„[klíčová věta nebo věrné shrnutí pravidla]"*
> — GoAC Rulebook, str. [X], *[Název odstavce]*

**Pravidla pro citace:**
- Cituj přímo z rulebooku — ideálně klíčovou větu nebo dvě, které pravidlo definují
- Pokud jde o shrnutí (ne doslova), uveď to formulací „[shrnutí]"
- Vždy uveď stránku **a** název odstavce (např. „str. 37, *Dissipating Heat*")
- U tabulek uveď název tabulky a stránku (např. „str. 19, *Attack Modifiers Table*")
- Pokud odpověď pokrývá více pravidel, přidej citaci ke každému klíčovému bodu
- Citace patří za odpověď jako samostatný blok

## Klíčové pojmy (rychlý glosář)

- **MP** = Movement Points
- **PSR** = Piloting Skill Roll
- **ToHit / TN** = Target Number (čím nižší potřebuješ hodit, tím lepší zbraň — ale hážeš 2D6 a potřebuješ **dosáhnout nebo překročit** TN)
- **Gunnery Skill** = základní TN pro střelbu (průměr: 4)
- **Piloting Skill** = základní TN pro PSR a fyzické útoky (průměr: 5)
- **GoAC** = "A Game of Armored Combat" — introductory ruleset (6 fází, jen BattleMechs)
- **IS** = Inner Sphere
