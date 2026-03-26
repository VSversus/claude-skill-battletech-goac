# Boj (Combat) — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Line of Sight | 13–14 |
| Firing Arcs | 14–15 |
| Attack Declaration / Torso Twists / Flipping Arms | 15 |
| Firing Weapons / GATOR | 15–16 |
| Target Number Modifiers (Attack Modifiers Table) | 16–19 |
| Combat in Water | 19 |
| Prone 'Mechs (střelba) | 19 |
| Specialized Attacks (Aimed Shot) | 21 |
| Rolling to Hit | 21 |
| Ammunition Expenditure | 21 |

---

## Přímá viditelnost (Line of Sight — LOS)

### Základní pravidla
- LOS se určuje ze středu hexu útočníka do středu hexu cíle
- LOS blokuje terén **mezi** hexem útočníka a cílem (krajní hexy se nepočítají)
- Potřebuješ LOS na **jakoukoliv** část cíle (pokud není cíl za kopcem)

### Úrovně a výška
- Mech stojí na úrovni svého hexu + 2 levely (Level 2 = výška mechu ~12 m)
- Terén blokuje LOS, pokud je vyšší než útočník nebo cíl
- Kopec blokuje LOS, pokud je mech na nižší úrovni

### Intervening Terrain (co blokuje LOS)
| Terén | Blokující podmínka |
|-------|-------------------|
| Light Woods | 3 a více consecutive hexů |
| Heavy Woods | 1× Light + 1× Heavy, nebo 2× Heavy |
| 2 hexy (kombinace) | viz tabulka v `tables.md` |

### Intervening Mechs
- Mech v intervening hexu blokuje LOS, pokud je ve stejné nebo vyšší výškové vrstvě
- Blokuje jak přátelské, tak nepřátelské mchy

### Water Hexes
- Mech v Depth 1 water: torzo je nad vodou (LOS k torzu stále možná)
- Mech v Depth 2+ water: plně ponořen; nelze na něj střílet ani z něj střílet

## Palebné oblouky (Firing Arcs)

### Standardní oblouky
- **Forward Arc**: 3 hexsides vpřed (fronty)
- **Left Side Arc**: 2 hexsides vlevo
- **Right Side Arc**: 2 hexsides vpravo
- **Rear Arc**: 1 hexside vzadu

Většina zbraní palí z **Forward Arc**. Některé zbraně mají jiné umístění (viz `weapons-equipment.md`).

### Torso Twist
- Deklaruje se při deklaraci útoku
- Otočí torso o 1–2 hexsides vlevo nebo vpravo
- Posune palebné oblouky zbraní v torsu (ne v pažích/nohách)
- Torso se vrátí do výchozí polohy na konci End fáze
- Modifikátor útoku: žádný dodatečný (pohybový modifikátor se nemění)

### Reversing (Flipping) Arms
- Deklaruje se při deklaraci útoku
- Otočí paže dozadu → zbraně v pažích mohou střílet do Rear Arc
- Paže se vrátí do výchozí polohy na konci End fáze
- Podmínka: mech musí mít funkční Lower Arm Actuator a Hand Actuator v paži

## GATOR — postup útoku

**G** — Grab the base Target Number (= Gunnery Skill pilota)
**A** — Attacker Movement Modifier (dle pohybového módu)
**T** — Target Movement Modifier (dle hexů, které cíl přešel)
**O** — Other Modifiers (vzdálenost, terén, specifické situace)
**R** — Roll 2D6; dosáhni nebo překroč TN

### Base Target Number
= Gunnery Skill pilota (průměr IS = 4)

### Attacker Movement Modifiers
| Pohybový mód | Modifikátor |
|-------------|------------|
| Stojí | +0 |
| Chůze | +1 |
| Běh | +2 |
| Skok | +3 |

### Target Movement Modifiers
Viz **Attack Modifiers Table** v `tables.md` (závisí na počtu hexů přešlých cílem).

### Other Modifiers — Range
| Vzdálenost | Modifikátor |
|-----------|------------|
| Short Range | +0 |
| Medium Range | +2 |
| Long Range | +4 |
| Minimum Range (pod min. range) | +(min range – vzdálenost), min +1 |
| Mimo max. range | Nelze střílet |

### Other Modifiers — Terrain
| Situace | Modifikátor |
|---------|------------|
| Partial Cover (Depth 1 water target) | +3 |
| Cíl v Light Woods | +1 |
| Cíl v Heavy Woods | +2 |
| Útočník v Light Woods | +1 |
| Útočník v Heavy Woods | +2 |
| Cíl je Prone + útok z boku/zadu | +0 |
| Cíl je Prone + útok zepředu | +1 |
| Cíl je Prone + útok z boku (vzdálenost 1) | −2 |
| Cíl je immobilní | −4 |

### Speciální situace
- **Prone attacker**: +2 modifikátor pro střelbu
- **Aimed shot** (viz níže)

## Boj ve vodě
- Mech v Depth 1: střelba normálně (ohnivé zbraně mají modifikátor)
- Mech v Depth 2+: nelze střílet (plně ponořen)
- Střelba na cíl v Depth 1: +3 (Partial Cover)

## Prone mechs ve střelbě
- Střílet lze jen z pozice prone
- +2 modifikátor útočníka (prone)
- Cíl prone: viz tabulka výše

## Speciální útoky

### Aimed Shot (cílený výstřel)
- Dostupný pouze pokud je cíl **immobilní**
- Deklaruje se při deklaraci útoku; útočník si vybere konkrétní lokaci
- Modifikátor: +3 ke stávajícímu TN (bonus za přesné míření = pevné umístění)
- Zabraňuje normálnímu hodu na hit location — místo toho se automaticky trefí do deklarované lokace

### Swarm/Streak/Artemis (v GoAC nejsou; jsou součástí Total Warfare)
V GoAC jsou pouze standardní LRM/SRM bez těchto vylepšení.

## Rozeznání útoku (Rolling to Hit)
1. Vypočítej výsledný TN (GATOR)
2. Hoď 2D6
3. Výsledek ≥ TN → zásah; výsledek < TN → minutí
4. Při zásahu: určení hit location → aplikace poškození

## Spotřeba munice
- Každý výstřel ze zbraně s municí spotřebuje 1 dávku munice
- Rakety: 1 výstřel = celý svazek (viz počet raket na výstřel)
- Dojde-li munice → zbraň nelze použít; žádný výbuch (pokud není crit do muničního slotu)

## Deklarace a pořadí
- Vždy nejprve **vše deklarovat**, pak **vše rozeznávat**
- Pořadí rozeznávání: poražený v iniciativě začíná
- Uvnitř jednoho mechu: hráč si volí pořadí zbraní
- Každý zásah plně rozeznán před dalším

---

## Klíčové citace — Combat

> 📖 *„The base Target Number for a weapon attack is equal to the attacker's Gunnery Skill Rating."*
> — GoAC Rulebook, str. 16, *Base Target Number (Gunnery Skill)*

> 📖 *„The attacker's Target Number is modified by their own movement using the values in the Attack Modifiers Table. The attacker's movement modifier is based on the movement mode it used in the turn (Walking, Running, or Jumping), not the actual MP expended or distance moved."*
> — GoAC Rulebook, str. 16, *Attacker Movement Modifier*

> 📖 *„A moving target is harder to hit [...]. The target movement modifier (often abbreviated as 'TMM') is based on the number of hexes traversed by the target this turn, not the number of Movement Points it spent."*
> — GoAC Rulebook, str. 16, *Target Movement Modifier*

> 📖 *„If a target jumped this turn, an attacker must also apply a +1 modifier to the attack's Target Number, in addition to the modifier for the number of hexes the target moved."*
> — GoAC Rulebook, str. 16, *Target Movement Modifier*

> 📖 *„Target Number modifiers due to heat never apply to physical attacks."*
> — GoAC Rulebook, str. 16, *Heat Modifier*

> 📖 *„A straight line running from the center of the attacker's hex to the center of the target's hex defines the LOS between two 'Mechs. [...] LOS is always mutual."*
> — GoAC Rulebook, str. 13, *Line of Sight*

> 📖 *„Players may announce that they are aiming for a specific hit location when declaring a weapon attack, but only against immobile targets. [...] Missiles cannot make an aimed shot."*
> — GoAC Rulebook, str. 21, *Aimed Shot*

> 📖 *„Each shot in a missile attack contains multiple projectiles. [...] The attacker determines how many of the missiles hit the target by rolling 2D6 and consulting the Cluster Hits Table."*
> — GoAC Rulebook, str. 24, *Missile Attacks*
