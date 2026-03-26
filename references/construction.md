# Stavba BattleMechu (Construction) — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| BattleMech Basics (Weight, Slots) | 49 |
| Step 1: Design the Chassis | 50–51 |
| Step 2: Install Engine | 51 |
| Step 3: Add Jump Jets | 51 |
| Step 4: Install Control Systems | 52 |
| Step 5: Add Armor | 52–53 |
| Step 6: Add Additional Heat Sinks | 53 |
| Step 7: Add Weapons and Ammunition | 54 |
| Step 8: Complete the Record Sheet | 54 |
| Weapons and Equipment Table | 55 |

---

## Základy (BattleMech Basics)

### Tonnage (Hmotnostní kategorie)
| Kategorie | Tonnage |
|----------|---------|
| Light | 20–35 t |
| Medium | 40–55 t |
| Heavy | 60–75 t |
| Assault | 80–100 t |

### Space (Slots)
Každá lokace má omezený počet slotů pro vybavení:
| Lokace | Počet slotů |
|--------|------------|
| Head | 6 |
| Center Torso | 12 |
| Left/Right Torso | 12 |
| Left/Right Arm | 12 |
| Left/Right Leg | 6 |

Část slotů je vždy obsazena povinnými komponentami (engine, gyro, cockpit, aktuátory).

## Krok za krokem (8 kroků)

### Krok 1: Design the Chassis

**Vyber tonnage** (20–100 tun, vždy násobek 5)

**Internal Structure**:
- IS = ⌈tonnage × 0,1⌉ za každou lokaci (přibližně; viz IS tabulka v `tables.md`)
- IS je pevně daná hodnotou dle tonnage
- Zaujímá sloty: viz tabulku níže

**Internal Structure Slots (per location)**:
- All Mechs: 1 slot v Head, 2× sloty v CT (dle váhy), atd.
- IS zabírá pevný počet slotů dle váhy mechu

**Aktuátory**:
- Paže: Shoulder + Upper Arm (povinné), Lower Arm + Hand (volitelné)
- Nohy: Hip + Upper Leg + Lower Leg + Foot (vše povinné)

### Krok 2: Install Engine

**Rating enginu** = Walking MP × tonnage mechu

Příklady:
| Walk MP | Tonnage | Engine Rating | Engine Tonnage |
|---------|---------|--------------|----------------|
| 3 | 50t | 150 | 5,5 t |
| 4 | 50t | 200 | 8,5 t |
| 5 | 50t | 250 | 12,5 t |
| 3 | 75t | 225 | 10 t |

Engine zabírá vždy **6 slotů** v Center Torso + po 3 sloty v každém side torsu (= 12 slotů celkem, pokud Xl/Light engine).

*Standard engine: 6 slotů v CT pouze.*

### Krok 3: Add Jump Jets
- Jump Jets = Jumping MP (max. = Walking MP)
- Každý JJ: 1 tuna (do 55t mechu) nebo 2 tuny (60t+)
- Sloty: 1 slot/JJ v noze nebo torsu

### Krok 4: Install Control Systems

**Gyroscope**:
- 4 sloty v Center Torso
- Tonnage: ⌈(engine rating ÷ 100)⌉ tuny

**Cockpit**:
- 1 slot v Head (+ Life Support a Sensors)
- Celkem Head využití: Cockpit (1) + Life Support (2) + Sensors (2) = 5 slotů + 1 free

### Krok 5: Add Armor

**Maximum armor** per lokace = 2 × IS hodnota lokace (Head = max 9)

**Armor tonnage**: každé 2 body pancíře = 1 tuna
- Přesněji: armor tonnage = celkové body pancíře ÷ 16 (zaokrouhlit nahoru)

**Přední vs. zadní armor** (pro torsa):
- Torsa mají přední i zadní pancíř
- Zadní pancíř min. 1 bod
- Přední + zadní ≤ max

### Krok 6: Add Additional Heat Sinks

Základní heat sinks jsou zabudovány v enginu:
- Engine Rating ÷ 25 = počet zabudovaných heat sinků (min 10)
- Každý extra heat sink: 1 tuna + 1 slot (kamkoliv je místo)

### Krok 7: Add Weapons and Ammunition

- Vyber zbraně a vybavení dle zbývající tonnage a slotů
- Každá zbraň má tonnage a počet slotů (viz `weapons-equipment.md`)
- Munice: 1 tuna = definovaný počet dávek

### Krok 8: Complete the Record Sheet

**Placing Items**:
1. Zakresli IS a armor hodnoty
2. Rozmisti všechny komponenty do slotů Critical Hit Table
3. Zaznamenej zbraně a jejich dostupy

**Final Steps**:
- Ověř celkovou tonnage (nesmí přesáhnout limit mechu)
- Ověř celkový počet slotů v každé lokaci
- Vyplň Heat Data (počet heat sinků)
- Nastav Heat Scale

## Weapons and Equipment Table — Tonnage/Sloty

| Zbraň/Vybavení | Tuny | Sloty |
|---------------|------|-------|
| Small Laser | 0,5 | 1 |
| Medium Laser | 1 | 1 |
| Large Laser | 5 | 2 |
| PPC | 7 | 3 |
| Flamer | 1 | 1 |
| Machine Gun | 0,5 | 1 |
| AC/2 | 6 | 1 |
| AC/5 | 8 | 4 |
| AC/10 | 12 | 7 |
| AC/20 | 14 | 10 |
| Gauss Rifle | 15 | 7 |
| SRM 2 | 1 | 1 |
| SRM 4 | 2 | 1 |
| SRM 6 | 3 | 2 |
| LRM 5 | 2 | 1 |
| LRM 10 | 5 | 2 |
| LRM 15 | 7 | 3 |
| LRM 20 | 10 | 5 |
| Heat Sink | 1 | 1 |
| Jump Jet (≤55t) | 1 | 1 |
| Jump Jet (60t+) | 2 | 1 |

**Munice (vždy 1 tuna, 1 slot)**:
| Munice pro | Sloty |
|-----------|-------|
| Libovolná zbraň | 1 |

## BattleValue (BV) — orientační přehled
BV je systém pro balancování sil. Není součástí základního GoAC výpočtu, ale je uvedeno na record sheetech. Pro scénáře: vyváženost = přibližně stejné BV na obou stranách.
