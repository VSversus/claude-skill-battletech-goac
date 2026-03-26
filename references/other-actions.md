# Ostatní akce — PSR, Pád, Displacement, Poškození pilota

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Piloting Skill Rolls — Making PSR | 40 |
| Piloting Skill Roll Timing | 40 |
| Displacement / Domino Effect | 40–42 |
| Falling — Location / Facing After Fall | 42 |
| Falling Damage to 'Mech | 43 |
| Falling Damage to MechWarrior | 43 |
| Accidental Falls From Above | 44 |
| Damaging a MechWarrior | 44 |

---

## Piloting Skill Rolls (PSR)

### Kdy se hodí PSR
| Situace | Modifikátor k PSR TN |
|---------|---------------------|
| Vstup do Rubble | +0 |
| Vstup do Depth 1 water | −1 (snazší) |
| Vstup do Depth 2 water | +0 |
| Vstup do Depth 3+ water | +1 |
| Vstávání (Standing Up) | +0 |
| Running + crit do gyra | +0 |
| Running + crit do boků (hip) | +0 |
| Jumping + loss of leg | +0 |
| Jumping + crit gyro/hip/leg actuator | +0 |
| Přijatý charge útok | +2 |
| Přijatý kick | 0 |
| Přijatý punch | 0 |
| Přijatý DFA | +2 |
| Každých 20 poškození v jednom tahu | +1 za každých 20 |
| 1 Gyro crit | +3 |
| Hip crit | +2 |
| Foot Actuator crit | +1 |
| Dolní část nohy (Lower Leg) crit | +1 |
| Horní část nohy (Upper Leg) crit | +1 |

*Kompletní tabulka včetně Preexisting Damage modifikátorů: viz str. 41, Piloting Skill Roll Table*

**Base TN pro PSR** = Piloting Skill pilota (průměr IS = 5)
Výsledný TN = Base + všechny aktuální modifikátory (jsou kumulativní)

> 📖 *„Piloting Skill Rolls use the MechWarrior's Piloting Skill as the base Target Number. [...] all modifiers applied by other events which have already occurred in the same phase [and] all modifiers applied due to Preexisting Damage [...] are cumulative and apply to all rolls."*
> — GoAC Rulebook, str. 40, *Making Piloting Skill Rolls*

### Timing PSR
- PSR z **pohybu** (entering terrain atd.): **okamžitě** při vstupu do hexu
- PSR z **útoků** (weapon i physical phase): na **konci fáze** po všech útocích, se všemi modifikátory
- PSR z **displacement**: **okamžitě**, bez ohledu na fázi
- Consciousness Roll vždy předchází PSR, pokud nastávají zároveň

> 📖 *„Movement Phase: Piloting Skill Rolls required due to a movement action [...] are made immediately following the action. Attack Phases: Piloting Skill Rolls due to attacks [...] are made at the end of the phase the attacks occurred in. Displacement: Any PSR required due to displacement [...] happens immediately, regardless of the phase."*
> — GoAC Rulebook, str. 40, *Piloting Skill Roll Timing*

### Immobilní mech a PSR
- Automaticky selže (pokud není prone)

> 📖 *„'Mechs that are immobile or that have an unconscious warrior automatically fail any required PSRs, if they were standing."*
> — GoAC Rulebook, str. 40, *Piloting Skill Rolls*

## Displacement (odsunutí)

Nastane, pokud dva mchy skončí ve stejném hexu po:
- Charge útoku (cíl je odsunut)
- Push útoku (cíl je odsunut)
- DFA (cíl je odsunut)
- Falling domino efektu

### Postup displacement
1. Odsunutý mech je přesunut do hexu přímo za ním (ve směru tlaku/dopadu)
2. Pokud je cílový hex obsazen: **Domino Effect**
3. Pokud je cílový hex nedostupný (zeď, kraj mapy): odsunutý mech padá a utrpí extra poškození

### Domino Effect
- Odsunutý mech narazí do dalšího mechu v sousedním hexu
- Ten druhý mech je odsunut stejným směrem
- Pokračuje dokud: hex je volný, hex je nedostupný (= pád), nebo jsme mimo mapu

## Falling (pád)

### Kdy mech padá
- Neúspěšná PSR (za pohyb v terénu, po zásahu, atd.)
- DFA útok (útočník vždy padá)
- 2 Gyro crits → okamžitý pád + immobilní
- Noha blown off → okamžitý pád
- Forced 2+ levels dolů
- Domino efekt

### Location After a Fall
- Pokud padá při pohybu z jednoho hexu do druhého → padá v **cílovém hexu**
- Pokud padá kvůli útoku nebo jinému důvodu → padá v **hexu, kde stojí**

> 📖 *„When a 'Mech falls while moving from one hex to another, it falls in the hex it was moving into. If a fall occurs because of an attack or any other combat-related reason, the 'Mech falls in the hex it occupies."*
> — GoAC Rulebook, str. 42, *Location After a Fall*

### Facing After a Fall — str. 43
Hoď **1D6** a konzultuj tabulku v `tables.md`.

> 📖 *„To determine the 'Mech's facing after the fall and where the 'Mech takes damage, roll 1D6 and consult the Facing After Fall Table."*
> — GoAC Rulebook, str. 43, *Facing After a Fall*

### Falling Damage — mech (str. 43)
- Poškození = **⌈tonnage ÷ 10⌉ × (levely pádu + 1)**
- Výsledek se rozdělí do skupin po 5 bodech; každá skupina = samostatný hod na hit location
- Hit location: dle Facing After Fall Table (viz `tables.md`)
- Voda: poškození se **dělí 2** (zaokrouhlit dolů) pokud mech padá v Depth 1+ water

> 📖 *„A fall deals damage equal to 1 point for every 10 tons that the 'Mech weighs (rounding up), multiplied by the number of levels plus 1 that the 'Mech fell. Divide the damage into 5-point Damage Value groupings."*
> — GoAC Rulebook, str. 43, *Falling Damage to a 'Mech*

### Falling Damage — MechWarrior (str. 43)
Po každém pádu: hráč provede **druhou PSR** (tzv. "seat belt check"):
- TN = stejné modifikátory jako PSR která způsobila pád + **+1 za každý level nad 1 fallen**
- Pokud PSR **selže** → pilot utrpí 1 poškození
- Automatické poškození (bez hodu): mech byl immobilní, nebo TN > 12

> 📖 *„A player makes a second Piloting Skill Roll after every fall (often called a seat belt check). All modifiers applied to the PSR that caused the fall are applied to this second roll, with an additional +1 modifier applied to the Target Number for every level above 1 fallen. If the roll succeeds, the MechWarrior avoids taking damage. If the roll fails, the MechWarrior takes 1 point of damage."*
> — GoAC Rulebook, str. 43, *Falling Damage to a MechWarrior*

### Accidental Falls From Above
- Pokud mech padá z vyšší úrovně do hexu obsazeného jiným mechem
- Oba mchi utrpí poškození:
  - Mech dole: ⌈(tonnage padajícího ÷ 10)⌉ × levely pádu
  - Padající mech: ⌈(tonnage mechu dole ÷ 10)⌉
- Padající mech přistane v sousedním hexu (random direction)
- Obě piloti: extra 1 poškození

## Damaging a MechWarrior (poškození pilota)

### Zdroje poškození pilota (str. 44)
- **Head hit** (jakýkoliv zásah hlavy, i bez průniku pancíře): 1 poškození
- **Pád** (seat belt check selže nebo mech immobilní): 1 poškození
- **Ammunition explosion**: 2 poškození
- **Teplo** (pouze pokud Life Support utrpěl Critical Hit): 1–2 poškození/kolo dle heat levelu (viz `heat.md`)

⚠️ Cockpit crit = **smrt pilota** (ne 2 poškození), mech je zničen.

### Pilot Damage Table (str. 44)

Tabulka ukazuje **Consciousness Number** pro každou úroveň poškození (viz `tables.md`). Pilotní skilly se **nemění** — pilot funguje normálně až do bezvědomí nebo smrti.

| Celkové poškození | Stav |
|------------------|------|
| 1–5 | Vědomý (hoď Consciousness Roll) |
| 6 | **Smrt** |

⚠️ Poznámka: Pilot Damage Table na record sheetu ukazuje čísla pro Consciousness Rolls (3, 5, 7, 10, 11, Dead) — to jsou TN hodnoty pro hod, ne penalizace ke skillům.

### Consciousness Rolls (str. 44)
Hoď **okamžitě** při každém bodu poškození pilota. Hoď 2D6 ≥ Consciousness Number:

| Celkové poškození pilota | Consciousness Number (TN) |
|--------------------------|--------------------------|
| 1 | 3 |
| 2 | 5 |
| 3 | 7 |
| 4 | 10 |
| 5 | 11 |
| 6 | **Smrt** |

Pokud hod selže → pilot v **bezvědomí** (mech immobilní); další Consciousness Rolls v tomto tahu se nehazí.

### Bezvědomý pilot
- Mech je **immobilní**
- V End Phase každého kola: hod 2D6 na probuzení (TN = 3; vždy se probere nakonec)
- Při probuzení: plné funkce obnoveny

### Smrt pilota
- Head blown off
- Poškození pilota ≥ 6 **a** neúspěšný Consciousness Roll s TN 12+
- Mech je zničen (pilot mrtev)
