# Heat Management — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Heat Points / Building Up Heat | 37 |
| **Dissipating Heat (heat sinky)** | **37** |
| Recording Heat Build-Up | 37 |
| Effects of Heat — Movement | 38 |
| Effects of Heat — Weapon Attacks | 38 |
| Effects of Heat — Shutdown | 38 |
| Effects of Heat — Ammunition | 38 |
| Effects of Heat — Damage to MechWarriors | 39 |

---

## Heat Points — základy

### Generování heat

| Akce | Heat generováno |
|------|----------------|
| Chůze (Walking) | 1 |
| Běh (Running) | 2 |
| Skok (Jumping) | 1 za každý přeskočený hex; **minimum 3** |
| Vstávání (Standing Up) | 1 za každý pokus |
| Každá zbraň | Dle statistiky zbraně (viz `weapons-equipment.md`) |
| Engine crit (1×) | +5 navíc každé kolo |
| Engine crit (2×) | +10 navíc každé kolo |

> 📖 *„Walking generates 1 heat point, no matter how many MP the 'Mech expends or how many hexes it moves. Running generates 2 heat points. Jump jets generate 1 heat point per Jumping MP expended, with a minimum of 3 heat points."*
> — GoAC Rulebook, str. 37, *Movement Heat*

### Disipace heat

| Podmínka | Heat odebráno |
|----------|--------------|
| Každý Heat Sink (suchý) | −1 za kolo |
| Každý Heat Sink **ponořený ve vodě** | −2 za kolo (dvojnásobek) |
| Maximum bonusu z vody | max. −6 bodů navíc za kolo |

**Které heat sinky jsou ponořené:**
- **Depth 1 water** (stojí): ponořeny pouze heat sinky v **nohách**
- **Depth 2+ water** (stojí) nebo **Depth 1+ water** (prone): ponořeny **všechny** heat sinky včetně engine

> 📖 *„Each heat sink dissipates 1 heat point per turn. Water: Submerged heat sinks dissipate twice as much heat. A 'Mech standing in Depth 1 water has its leg-mounted heat sinks submerged. A 'Mech standing in Depth 2 or deeper water or prone in Depth 1 or deeper water has all of its heat sinks submerged (even those in the engine). No more than 6 additional heat points per turn can be dissipated due to water."*
> — GoAC Rulebook, str. 37, *Dissipating Heat*

**Standardní výchozí stav**: mech má 10 heat sinků; přesný počet je na record sheetu.

### Recording Heat Build-Up
- Heat Scale na record sheetu: od 0 do 30+ (Heat Overflow)
- Každé kolo: přičti generované heat → odečti disipaci → označ výsledek na Heat Scale
- Heat přetékající přes 30 → zaznamenat do "Heat Overflow" pole

> 📖 *„During each turn's Heat Phase, each player adds up the heat points built up by their 'Mech. They then subtract the heat dissipated by heat sinks. The result may be positive or negative. Add this number to the current level of heat shown on the Heat Scale."*
> — GoAC Rulebook, str. 37, *Recording Heat Build-Up*

## Efekty přehřátí (Effects of Heat)

Heat Timing: efekty nastávají **po** úpravě heat levelu v Heat Phase.

> 📖 *„The 'Mech suffers heat effects after players have adjusted the heat level for the turn as described above in Recording Heat Build-up."*
> — GoAC Rulebook, str. 38, *Effects of Heat*

### Pohyb (Movement) — str. 38
| Heat Level | Efekt na Walking MP |
|-----------|---------------------|
| 5 | −1 MP |
| 10 | −2 MP |
| 15 | −3 MP |
| 20 | −4 MP |
| 25 | −5 MP |

*Efekty nejsou kumulativní — vždy platí jen ten pro aktuální heat level.*
*Running MP se recalkuluje z nového Walking MP (× 1,5 zaokrouhlit nahoru).*
*Jumping MP teplem ovlivněn není.*

> 📖 *„This effect is not cumulative with any previous heat-caused Movement Point loss. For example, when a 'Mech's heat build-up reaches 5 on the Heat Scale, its Walking MP is reduced by 1. When the build-up reaches 10 on the Heat Scale, reduce Walking MP by 2 total, not by 2 more MP. Jumping: Reductions in Walking MP from heat build-up do not affect a 'Mech's Jumping MP."*
> — GoAC Rulebook, str. 38, *Movement*

### Střelba (Weapon Attacks) — str. 38
| Heat Level | Modifikátor k weapon attacks |
|-----------|------------------------------|
| 8–12 | +1 |
| 13–16 | +2 |
| 17–23 | +3 |
| 24+ | +4 |

*Netýká se fyzických útoků.*

> 📖 *„At 8, 13, 17, and 24 heat points, add the number indicated to the 'Mech's Target Number for weapon attacks. [...] These penalties apply only to weapon attacks, not physical attacks."*
> — GoAC Rulebook, str. 38, *Weapon Attacks*

### Shutdown — str. 38
| Heat Level | Efekt |
|-----------|-------|
| 14 | Hod 2D6, potřeba ≥ 4 (Avoid on 4+) nebo shutdown |
| 18 | Hod 2D6, potřeba ≥ 6 (Avoid on 6+) nebo shutdown |
| 22 | Hod 2D6, potřeba ≥ 8 (Avoid on 8+) nebo shutdown |
| 26 | Hod 2D6, potřeba ≥ 10 (Avoid on 10+) nebo shutdown |
| 30 | **Automatický Shutdown** (nelze se vyhnout) |

*Pokud heat dosáhne více trigger úrovní najednou → hod jen jednou proti nejvyššímu TN.*
*Pokud shutdown nastane → okamžitá PSR s modifikátorem +3.*

> 📖 *„At 14, 18, 22, 26, and 30 heat points, a 'Mech attempts to shut down its power plant automatically [...]. If heat accumulation reaches two or more trigger levels in one turn, roll 2D6 only once, against the highest Avoid Target Number. If a 'Mech shuts down, a Piloting Skill Roll is immediately required, with a +3 Target Number modifier."*
> — GoAC Rulebook, str. 38, *Shutdown*

**Voluntary Shutdown**: hráč může dobrovolně shut down v End Phase; restart v libovolném dalším End Phase (musí nejprve projít Shutdown Avoid check dle aktuálního heat levelu).

**Restart po nuceném shutdown**: každá Heat Phase se pokusí o restart; TN = nejvyšší aktuální Avoid Target Number; heat musí být pod 30.

> 📖 *„Players may elect to voluntarily shut down a 'Mech during any End Phase. They may then restart the power plant in any subsequent End Phase, provided they first pass any Shutdown Avoid checks due to heat (if needed). Overflow Heat: A 'Mech's heat level must be below 30 before a restart can occur."*
> — GoAC Rulebook, str. 38, *Voluntary Shutdown*

### Muniční exploze (Ammunition) — str. 38
| Heat Level | Efekt |
|-----------|-------|
| 19–22 | Hod 2D6, potřeba ≥ 4 (Avoid on 4+), jinak exploze |
| 23–27 | Hod 2D6, potřeba ≥ 6 (Avoid on 6+), jinak exploze |
| 28–30 | Hod 2D6, potřeba ≥ 8 (Avoid on 8+), jinak exploze |

Při explozi: exploze muniční slot s **nejvyšší hodnotou poškození za výstřel** (= Damage Value × shots). Hráč volí při shodě.

> 📖 *„If a 'Mech with unemptied bins of ammunition reaches 19 points or higher on the Heat Scale, one of these bins may explode. [...] When an overheated 'Mech's ammo explodes, the ammunition critical slot with the most destructive ammo per shot explodes first."*
> — GoAC Rulebook, str. 38, *Ammunition*

### Poškození pilota teplem — str. 39
⚠️ **Toto nastane pouze pokud mech utrpěl Critical Hit na Life Support!** Bez critu teplo pilota nezraňuje.

| Heat Level (při critu Life Support) | Poškození pilota |
|------------------------------------|-----------------|
| 15–25 | 1 poškození za kolo |
| 26+ | 2 poškození za kolo |

> 📖 *„If a 'Mech's life support system takes one or more critical hits, its MechWarrior suffers damage when the 'Mech's heat levels are high. The MechWarrior takes 1 point of damage (wound) at the end of every Heat Phase that the 'Mech's Heat Scale is between 15 and 25; if the Heat Scale is 26 or higher, the MechWarrior takes 2 points of damage instead."*
> — GoAC Rulebook, str. 39, *Damage to MechWarriors*

## Shutdown — detailně

### Nucený Shutdown
- Nastane při dosažení trigger heat úrovně a neúspěšném Avoid hozu
- Shutdown mech je **immobilní**; žádná akce není možná
- Výjimka: heat sinky a life support fungují i při shutdown
- Engine crits negenerují heat při shutdown
- Okamžitá PSR s modifikátorem +3 při shutdownu

> 📖 *„Additionally, the 'Mech becomes immobile. Its equipment ceases to function except for heat sinks and life support, and it cannot attack or take any other action. Engine critical hits do not generate heat while a 'Mech is shut down."*
> — GoAC Rulebook, str. 38, *Shutdown*

### Voluntary Shutdown
- Deklaruje se v End Phase
- Restart: v libovolném dalším End Phase (hod na Avoid dle aktuálního heat levelu)
- Mech může jednat od **tahu následujícího** po restartu

### Restart (nucený i dobrovolný)
- TN = aktuální nejvyšší Avoid Target Number pro daný heat level
- Heat musí být pod 30 před restartem
- Pokud heat klesne pod 14 → automatický restart (i bez vědomého pilota)

> 📖 *„When the heat drops below 14 on the Heat Scale, the power plant restarts automatically, even if the pilot is out of action."*
> — GoAC Rulebook, str. 38, *Shutdown*
