# Zbraně a vybavení (Weapons & Equipment) — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Weapons and Equipment Table | 55 |
| Weapons and Equipment (popis jednotlivých zbraní) | 56+ |

---

## Jak číst statistiku zbraně

```
Název | Lokace | Heat | Damage | Type | Min | Short | Medium | Long
```

- **Lokace**: kde je zbraň na record sheetu (LA=Left Arm, RA=Right Arm, LT=Left Torso, RT=Right Torso, CT=Center Torso, LL=Left Leg, RL=Right Leg, HD=Head)
- **Heat**: teplo generované při výstřelu
- **Damage**: poškození při zásahu
- **Type**: DE = Direct Energy (laser), DB = Direct Ballistic (kulomety/kanóny), M = Missile, C = Cluster
- **Min/Short/Medium/Long**: dostřely v hexech

## Zkratky typů zbraní
- **[DE]**: Direct Energy — laser, PPC; žádná munice
- **[DB,S]**: Direct Ballistic, Single — kulomety, AC; munice
- **[M,C,S]**: Missile, Cluster, Single — rakety (LRM/SRM)

## Základní zbraně GoAC

### Energy Weapons (bez munice)

| Zbraň | Heat | Dmg | Min | Short | Medium | Long |
|-------|------|-----|-----|-------|--------|------|
| Small Laser | 1 | 3 | — | 1 | 2 | 3 |
| Medium Laser | 3 | 5 | — | 3 | 6 | 9 |
| Large Laser | 8 | 8 | — | 5 | 10 | 15 |
| PPC | 10 | 10 | 3 | 6 | 12 | 18 |
| Flamer | 3 | 2* | — | 1 | 2 | 3 |

*Flamer: +2 heat cíli (místo normálního damage; lze volit)

### Ballistic Weapons (potřebují munici)

| Zbraň | Heat | Dmg | Min | Short | Medium | Long |
|-------|------|-----|-----|-------|--------|------|
| Machine Gun | 0 | 2 | — | 1 | 2 | 3 |
| AC/2 | 1 | 2 | 4 | 8 | 16 | 24 |
| AC/5 | 1 | 5 | 3 | 6 | 12 | 18 |
| AC/10 | 3 | 10 | — | 5 | 10 | 15 |
| AC/20 | 7 | 20 | — | 3 | 6 | 9 |
| Gauss Rifle | 1 | 15 | 2 | 7 | 15 | 22 |

### Missile Weapons (potřebují munici)

| Zbraň | Heat | Dmg/raketa | Min | Short | Medium | Long |
|-------|------|-----------|-----|-------|--------|------|
| SRM 2 | 2 | 2/raketa | — | 3 | 6 | 9 |
| SRM 4 | 3 | 2/raketa | — | 3 | 6 | 9 |
| SRM 6 | 4 | 2/raketa | — | 3 | 6 | 9 |
| LRM 5 | 2 | 1/raketa | 6 | 7 | 14 | 21 |
| LRM 10 | 4 | 1/raketa | 6 | 7 | 14 | 21 |
| LRM 15 | 5 | 1/raketa | 6 | 7 | 14 | 21 |
| LRM 20 | 6 | 1/raketa | 6 | 7 | 14 | 21 |

### Speciální poznámky k raketám
- **Cluster Hits**: při zásahu hoď znovu 2D6 na Cluster Hits Table → zjisti kolik raket zasáhne (viz `tables.md`)
- Každá zasáhnuvší raketa způsobuje damage uvedené výše (LRM: 1/raketa; SRM: 2/raketa)
- **LRM hit locations**: rakety se aplikují ve skupinách po 5; každá skupina = 1 hod na hit location
- **SRM hit locations**: každá raketa = zvláštní hod na hit location
- Minimum range: pokud je cíl blíže než min. range → +1 TN za každý hex pod minimem

## Speciální pravidla zbraní

### PPC (Particle Projector Cannon)
- Minimum range 3 hexy: pokud cíl blíže → modifikátor (viz Range Modifiers v `tables.md`)
- Energie, žádná munice

### Flamér
- Místo normálního damage lze vybrat: způsobit cíli +2 heat navíc (per výstřel)
- Lze kombinovat: damage + heat? Záleží na verzi pravidel — v GoAC volba hráče

### Gauss Rifle
- **Pozor**: při critickém zásahu do Gauss Rifle → **exploduje** za 20 poškození (do mechu, který ji nese)
- V GoAC základní sadě nemusí být Gauss Rifle dostupný

## Munice (Ammunition)

### Kapacita munice (přibližně)
| Zbraň | Výstřelů na tunu munice |
|-------|------------------------|
| Machine Gun | 200 |
| AC/2 | 45 |
| AC/5 | 20 |
| AC/10 | 10 |
| AC/20 | 5 |
| SRM 2 | 50 (raket) |
| SRM 4 | 25 (raket) |
| SRM 6 | 15 (raket) |
| LRM 5 | 24 (raket) |
| LRM 10 | 12 (raket) |
| LRM 15 | 8 (raket) |
| LRM 20 | 6 (raket) |

### Ammo Explosion
- Critical hit do muničního slotu → **okamžitá exploze**
- Poškození = počet zbývajících dávek munice
- 1 dávka = 1 damage (Machine Gun), nebo 1 výstřel (rakety/AC)
- Hit location: do Center Torso (nebo dle specifické situace)

## Vybavení (Equipment)

### Heat Sinks
- Každý Heat Sink: disipuje 1 heat point za kolo
- Standardní mech = 10 heat sinků (zabudováno v engine)
- Každé 2 tuny navíc = 1 extra heat sink

### Jump Jets
- 1 tuna za každý Jumping MP do 55t
- 2 tuny za každý Jumping MP od 60t+
- Umístěny v nohách nebo torsu

### Cockpit
- 1 slot v Head

### Gyroscope
- 4 sloty v Center Torso

### Engine
- Různé velikosti; velikost = Walking MP × tonnage

## Fyzické zbraně (Physical Weapons — rozšíření)
V základním GoAC rulekooku tyto nejsou; vyskytují se v Total Warfare a BattleMech Manual:
- **Hatchet**: +1 damage oproti punch, specifické sloty
- **Sword**: podobné jako Hatchet
- **Mace**: těžší, pomalejší

## Poznámky pro hru
- Vždy zkontroluj record sheet konkrétního mechu pro přesné statistiky
- GoAC obsahuje základní sadu mechů — jejich statistiky jsou na přiložených record sheetech
- Pro vybavení mimo GoAC rozsah: viz Total Warfare nebo BattleMech Manual
