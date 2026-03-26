# Tabulky (Tables) — GoAC — Kompletní Reference

## Attack Modifiers Table (Modifikátory k útoku)

### Attacker Movement Modifier
| Pohybový mód | Modifikátor |
|-------------|------------|
| Stojí | +0 |
| Chůze | +1 |
| Běh | +2 |
| Skok | +3 |

### Target Movement Modifier (dle hexů přešlých cílem)
| Hexů přešel cíl | Modifikátor |
|----------------|------------|
| 0 (stojí/immobilní) | +0 |
| 1–2 | +1 |
| 3–4 | +2 |
| 5–6 | +3 |
| 7–9 | +4 |
| 10–17 | +5 |
| 18–24 | +6 |
| 25+ | +7 |

Cíl, který **skočil**: přičti +1 navíc k hodnotě dle hexů.

### Range Modifiers
| Vzdálenost | Modifikátor |
|-----------|------------|
| Short | +0 |
| Medium | +2 |
| Long | +4 |
| Minimum (pod min. range) | +(min range − vzdálenost) |

### Terrain Modifiers (Útočník/Cíl)
| Situace | Modifikátor |
|---------|------------|
| Útočník v Light Woods | +1 |
| Útočník v Heavy Woods | +2 |
| Cíl v Light Woods | +1 |
| Cíl v Heavy Woods | +2 |
| Cíl v Depth 1 water (Partial Cover) | +3 |
| Cíl je Prone (z boku/zadu) | +0 |
| Cíl je Prone (zepředu) | +1 |
| Cíl je Prone (vzdálenost 1, bok) | −2 |
| Cíl je immobilní | −4 |
| Aimed Shot (immobilní cíl) | +3 (ale vybereš lokaci) |

### Other Modifiers
| Situace | Modifikátor |
|---------|------------|
| Útočník je prone (střelba z pole) | +2 |
| Senzory (1 crit) | +1 |
| Senzory (2 crits) | +2 |
| Heat 8 | +1 |
| Heat 13 | +2 |
| Heat 17 | +3 |
| Heat 24 | +4 |

---

## Hit Location Tables (2D6)

### Přední útok (Front Attack)

| 2D6 | Lokace |
|-----|--------|
| 2 | Center Torso (Critical) |
| 3 | Right Arm |
| 4 | Right Arm |
| 5 | Right Leg |
| 6 | Right Torso |
| 7 | Center Torso |
| 8 | Center Torso |
| 9 | Left Torso |
| 10 | Left Leg |
| 11 | Left Arm |
| 12 | Head |

### Levý boční útok (Left Side Attack)

| 2D6 | Lokace |
|-----|--------|
| 2 | Left Torso (Critical) |
| 3 | Left Leg |
| 4 | Left Arm |
| 5 | Left Arm |
| 6 | Left Leg |
| 7 | Left Torso |
| 8 | Center Torso |
| 9 | Right Torso |
| 10 | Right Arm |
| 11 | Right Leg |
| 12 | Head |

### Pravý boční útok (Right Side Attack)

| 2D6 | Lokace |
|-----|--------|
| 2 | Right Torso (Critical) |
| 3 | Right Leg |
| 4 | Right Arm |
| 5 | Right Arm |
| 6 | Right Leg |
| 7 | Right Torso |
| 8 | Center Torso |
| 9 | Left Torso |
| 10 | Left Arm |
| 11 | Left Leg |
| 12 | Head |

### Zadní útok (Rear Attack)

| 2D6 | Lokace |
|-----|--------|
| 2 | Center Torso (Rear, Critical) |
| 3 | Right Arm |
| 4 | Right Arm |
| 5 | Right Leg |
| 6 | Right Torso (Rear) |
| 7 | Center Torso (Rear) |
| 8 | Center Torso (Rear) |
| 9 | Left Torso (Rear) |
| 10 | Left Leg |
| 11 | Left Arm |
| 12 | Head |

---

## Critical Hits Table (2D6)

| 2D6 | Výsledek |
|-----|---------|
| 2–7 | Žádný Critical Hit |
| 8–9 | 1 Critical Hit |
| 10–11 | 2 Critical Hits |
| 12 | 3 Critical Hits |

---

## PSR Modifiers Table

| Situace | Modifikátor k PSR TN |
|---------|---------------------|
| Přijat kick | +2 |
| Přijat punch | +0 |
| Každých 20 poškození v jedné fázi | +1 za každých 20 |
| 1 Gyro crit | +3 |
| Hip crit | +2 |
| Foot Actuator crit | +1 |
| Lower Leg Actuator crit | +1 |
| Upper Leg Actuator crit | +1 |

---

## Consciousness Roll Table — str. 44

Hoď okamžitě při každém bodu poškození. Hod 2D6 ≥ Consciousness Number → pilot vědomý.

| Poškození pilota | Consciousness Number |
|-----------------|---------------------|
| 1 | 3 |
| 2 | 5 |
| 3 | 7 |
| 4 | 10 |
| 5 | 11 |
| 6 | **Smrt** |

---

## Cluster Hits Table — Počet zasáhnuvších raket (2D6)

**Postup:** Nejprve hoď na to-hit. Při zásahu hoď **znovu 2D6** a zjisti z tabulky, kolik raket skutečně zasáhne. Pak hoď hit location pro každou skupinu raket (LRM: skupiny po 5; SRM: každá raketa zvlášť).

| 2D6 | SRM 2 | SRM 4 | SRM 6 | LRM 5 | LRM 10 | LRM 15 | LRM 20 |
|-----|-------|-------|-------|-------|--------|--------|--------|
| 2   | 1     | 1     | 2     | 1     | 3      | 5      | 6      |
| 3   | 1     | 2     | 2     | 2     | 3      | 5      | 6      |
| 4   | 1     | 2     | 3     | 2     | 4      | 6      | 9      |
| 5   | 1     | 2     | 3     | 3     | 6      | 9      | 12     |
| 6   | 1     | 3     | 3     | 3     | 6      | 9      | 12     |
| 7   | 1     | 3     | 3     | 3     | 6      | 9      | 12     |
| 8   | 2     | 3     | 3     | 3     | 6      | 9      | 12     |
| 9   | 2     | 3     | 4     | 4     | 8      | 12     | 16     |
| 10  | 2     | 3     | 4     | 4     | 8      | 12     | 16     |
| 11  | 2     | 4     | 5     | 5     | 10     | 15     | 20     |
| 12  | 2     | 4     | 5     | 5     | 10     | 15     | 20     |

**Poznámky:**
- Průměrný hod 7 zasáhne ~60 % raket (LRM) nebo 50–75 % (SRM)
- LRM damage: každá raketa = 1 poškození; LRM skupiny jsou po 5 → každá skupina = 1 hod na hit location
- SRM damage: každá raketa = 2 poškození; každá raketa = zvláštní hod na hit location
- Artemis IV FCS (rozšíření, ne GoAC): +2 k cluster hozu
- NARC beacon (rozšíření): +2 k cluster hozu

---

## Movement Costs Table (přehled — viz `movement.md` pro full verzi)

| Terén | MP cena | PSR |
|-------|---------|-----|
| Základ (jakýkoliv hex) | 1 | — |
| Clear | +0 | — |
| Rough | +1 | — |
| Light Woods | +1 | — |
| Heavy Woods | +2 | — |
| Water Depth 1 | +1 | Ano (−1) |
| Water Depth 2+ | +3 | Ano |
| Rubble | +1 | Ano (+0) |
| Level change (1) | +1 | — |
| Level change (2) | +2 | — |
| Facing change | 1/hexside | — |
| Stand up | 2/pokus | Ano |

---

## Pilot Damage Table — str. 44

Pilot skilly se nemění. Tabulka na record sheetu = Consciousness Numbers pro hody.

| Poškození | Stav |
|-----------|------|
| 1–5 | Vědomý (hoď Consciousness Roll po každém bodu) |
| 6 | Smrt |

---

## Heat Effects Summary — str. 38–39

| Heat | Pohyb (Walking MP) | Střelba | Shutdown / Ammo / Life Support |
|------|-------------------|---------|-------------------------------|
| 5 | −1 MP | — | — |
| 8–12 | — | +1 | — |
| 10 | −2 MP | — | — |
| 13–16 | — | +2 | — |
| 14 | — | — | Shutdown, avoid on 4+ |
| 15 | −3 MP | — | (Life Support crit: 1 dmg/kolo) |
| 17–23 | — | +3 | — |
| 18 | — | — | Shutdown, avoid on 6+ |
| 19–22 | — | — | Ammo exploze, avoid on 4+ |
| 20 | −4 MP | — | — |
| 22 | — | — | Shutdown, avoid on 8+ |
| 23–27 | — | — | Ammo exploze, avoid on 6+ |
| 24+ | — | +4 | — |
| 25 | −5 MP | — | — |
| 26 | — | — | Shutdown, avoid on 10+; (Life Support crit: 2 dmg/kolo) |
| 28–30 | — | — | Ammo exploze, avoid on 8+ |
| 30 | — | — | **Automatický Shutdown** |

*Pohybové efekty nejsou kumulativní — vždy platí jen jeden (ten pro aktuální level).*
*Střelecké efekty také nejsou kumulativní.*
*Life Support sloupec: platí pouze při Critical Hitu na Life Support komponentu.*

---

## Facing After a Fall Table (1D6) — str. 43

| 1D6 | Nová orientace | Hit Location Column |
|-----|---------------|---------------------|
| 1 | Beze změny (Same Direction) | Front |
| 2 | 1 hexside doprava | Right Side |
| 3 | 2 hexsidy doprava | Right Side |
| 4 | Čelem vzad (Opposite Direction) | Rear |
| 5 | 2 hexsidy doleva | Left Side |
| 6 | 1 hexside doleva | Left Side |

---

## Internal Structure Values (Standard)

| Tonnage | Head | CT | LT/RT | LA/RA | LL/RL |
|---------|------|----|-------|-------|-------|
| 20t | 3 | 6 | 5 | 3 | 4 |
| 25t | 3 | 8 | 6 | 4 | 6 |
| 30t | 3 | 10 | 7 | 5 | 7 |
| 35t | 3 | 11 | 8 | 6 | 8 |
| 40t | 3 | 12 | 10 | 6 | 10 |
| 45t | 3 | 14 | 11 | 7 | 11 |
| 50t | 3 | 16 | 12 | 8 | 12 |
| 55t | 3 | 18 | 13 | 9 | 13 |
| 60t | 3 | 20 | 14 | 10 | 14 |
| 65t | 3 | 21 | 15 | 10 | 15 |
| 70t | 3 | 22 | 15 | 11 | 15 |
| 75t | 3 | 23 | 16 | 12 | 16 |
| 80t | 3 | 25 | 17 | 13 | 17 |
| 85t | 3 | 27 | 18 | 13 | 18 |
| 90t | 3 | 29 | 19 | 14 | 19 |
| 95t | 3 | 30 | 20 | 15 | 20 |
| 100t | 3 | 31 | 21 | 17 | 21 |

CT = Center Torso, LT/RT = Left/Right Torso, LA/RA = Left/Right Arm, LL/RL = Left/Right Leg
