# Poškození (Damage) — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Damage Resolution / Resolution Order / Timing | 30 |
| Critical Hits / Applying Critical Hits | 30–31 |
| Critical Hit Effects (přehled všech komponent) | 32–34 |
| Destroyed Locations | 34 |
| Transferring Damage | 34 |
| Destroying a 'Mech | 35 |
| Step-by-Step Damage | 35 |
| Hit Location Tables | 22–24 |

---

## Damage Resolution — pořadí

1. Urči **hit location** (hod 2D6 + útočníkův směr útoku → tabulka)
2. Odečti poškození od **pancíře** (Armor) dané lokace
3. Pokud pancíř nestačí: zbývající poškození jde do **Internal Structure** (IS)
4. Pokud IS vyčerpána: lokace je **zničena** → hod na Critical Hits
5. Poškození přes IS zničené lokace se **přenáší** (Transfer)

### Damage Timing
- Střelba: poškození se aplikuje **okamžitě** při rozeznávání (ne na konci fáze)
- Fyzické útoky: poškození se aplikuje **před** Heat Phase

## Hit Location

### Útočníkův směr (Attack Direction)
Závisí na orientaci cíle vůči útočníkovi:
- **Přední oblouk (Front)**: útočník je v předních 3 hexsidech cíle
- **Levý bok (Left Side)**: útočník je v levém bočním hexsidu
- **Pravý bok (Right Side)**: útočník je v pravém bočním hexsidu
- **Zadní (Rear)**: útočník je vzadu

### Hit Location Tables — viz `tables.md`
(Front, Left Side, Right Side, Rear — každý má vlastní tabulku 2D6 → lokace)

## Critical Hits

### Kdy nastává
Při **zničení lokace** (IS = 0):
- Každý další bod poškození do IS způsobuje hod na critical hits

### Through-Armor Critical (TAC)
Výjimka: hod **2** na Hit Location Table spustí crit check **i bez průniku pancíře**, pokud útok způsobil alespoň 1 bod poškození. Pancíř nemusí být proražen — samotný hod 2 stačí.

> 📖 *„A roll of 2 on the Hit Location Table provides a chance for a critical hit, even if the attack did not damage internal structure (though the attack must still have dealt at least 1 point of damage). This is known as a through-armor critical (TAC) hit."*
> — GoAC Rulebook, str. 31, *Through-Armor Critical Hit*

### Applying Critical Hits
1. Hoď 2D6:
   - 2–7: žádný crit
   - 8–9: 1 crit
   - 10–11: 2 crits
   - 12: 3 crits (nebo specifická destrukce)

2. Pro každý crit: hoď 1D6 (nebo 2D6 dle systému) na **slot** v dané lokaci z Critical Hit Table na record sheetu
   - Pokud slot je "Roll Again": hoď znovu
   - Pokud slot je prázdný (already destroyed): žádný efekt

### Ammo Explosion
- Pokud crit zasáhne muniční slot → **okamžitá exploze**
- Poškození: počet dávek munice (každá = 1 bod) nebo dle tabulky
- Hit location: hod na center torso (nebo specifická lokace dle typy munice)

## Critical Hit Effects — přehled

| Komponenta | Lokace | Efekt |
|-----------|--------|-------|
| Ammunition | Libovolná | Okamžitá exploze |
| Arm Blown Off | Paže | Paže zcela odletí |
| Cockpit | Hlava | Pilot zabit nebo omráčen (2 poškození pilota) |
| Engine | Torso | 1 crit: +5 heat/tah; 2 crits: +10 heat/tah; 3 crits: zničení |
| Foot Actuator | Noha | −1 k Walking MP; PSR při chůzi/běhu |
| Gyro | Torso | 1 crit: PSR při chůzi/běhu; 2 crits: mech padá, stane se immobilním |
| Hand Actuator | Paže | Nelze punch/push; −1 k fyzickému poškození |
| Head Blown Off | Hlava | Pilot zabit |
| Heat Sink | Torso/Noha | −1 k heat dissipation |
| Hip | Noha | Nelze běhat; −2 k Walking MP |
| Jump Jet | Noha/Torso | −1 k Jumping MP |
| Leg Blown Off | Noha | Noha zcela odletí; mech padá |
| Life Support | Hlava | Nelze přežít v ponoření (1 poškození pilota/tah v Depth 2+ water) |
| Lower Arm Actuator | Paže | Nelze flipovat paže; −1 k fyzickému poškození |
| Lower Leg Actuator | Noha | −1 k Walking MP; PSR při chůzi/běhu |
| Sensors | Hlava | 1 crit: +1 k veškerým útokům; 2 crits: +2 |
| Shoulder | Paže | Nelze provádět fyzické útoky tou paží; nelze flipovat |
| Upper Arm Actuator | Paže | Nelze flipovat paže |
| Upper Leg Actuator | Noha | −1 k Walking MP; PSR při chůzi/běhu |
| Weapons & Equipment | Libovolná | Zbraň/vybavení zničeno/nefunkční |

### Engine Crits (detailně)
- **1 Engine crit**: +5 heat generovaný každé kolo navíc
- **2 Engine crits**: +10 heat navíc
- **3 Engine crits**: mech je **zničen** (reactor exploduje)

### Gyro Crits (detailně)
- **1 Gyro crit**: každé použití Walking nebo Running MP → PSR; skok není možný
- **2 Gyro crits**: mech se stane **immobilním** a okamžitě padá

## Destroyed Locations (zničené lokace)

| Lokace | Efekt při zničení |
|--------|------------------|
| Head | Pilot zabit → mech zničen |
| Center Torso | Mech zničen |
| Left/Right Torso | Vybavení v lokaci zničeno; mech pokračuje |
| Left/Right Arm | Paže odletí; zbraně v paži zničeny |
| Left/Right Leg | Noha odletí; mech padá; specifická omezení pohybu |

### Jeden kritický hit při zničení
Při prvním zničení lokace vždy nastane **1 crit** (nezávisle na hodu výše).

## Transferring Damage (přenos poškození)

Pokud je IS lokace již zničena a dojde další poškození:
- Poškození se **přenáší** do sousední lokace dle Damage Transfer Diagrame

### Damage Transfer Diagram (standardní)
| Zdrojová lokace | Přenos do |
|----------------|-----------|
| Head | Center Torso |
| Left Arm | Left Torso |
| Right Arm | Right Torso |
| Left Torso | Center Torso |
| Right Torso | Center Torso |
| Left Leg | Left Torso |
| Right Leg | Right Torso |
| Center Torso | **Mech zničen** |

## Destroying a 'Mech — jak je mech zničen

Mech je zničen pokud:
1. **Center Torso** je zničen (IS = 0)
2. **Head** je zničena
3. **Engine** utrpí 3 kritické zásahy
4. **Kokpit** kritický zásah způsobí smrt pilota
5. Oba mče přijdou o všechny 4 končetiny (obě paže + obě nohy) → v GoAC je to zničení

## Step-by-Step Damage (krok za krokem)

```
1. Útok zasáhne → hod na hit location
2. Poškození - armor lokace
   a. Pokud armor > 0 → hotovo (zatím)
   b. Pokud armor = 0 → přejdi na IS
3. Zbývající poškození - IS lokace
   a. IS > 0 → hotovo (zatím)
   b. IS = 0 → lokace zničena → critical hit check
4. Critical hit check: 2D6 → 0/1/2/3 crits
   Pro každý crit: náhodný slot v lokaci
5. Poškození přes zničenou IS → Damage Transfer → přejdi na krok 2 pro novou lokaci
```

---

## Klíčové citace — Damage

> 📖 *„Damage from any source is first applied to the armor of the location damaged [...]. Once the armor of a location/facing is gone, any further damage to there is dealt to the internal structure of that location."*
> — GoAC Rulebook, str. 30, *Damage Resolution*

> 📖 *„It is also important to understand that, when applying damage, every single hit is completely resolved—both the damage dealt and any critical hits inflicted—before moving on to the next hit."*
> — GoAC Rulebook, str. 30, *Resolution Order*

> 📖 *„Damage dealt by attacks made in the Weapon Attack or Physical Attack Phases [...] is resolved as it happens. However, damage dealt by attacks never affects any other attack made in the same phase. All attacks declared in a phase get to be made."*
> — GoAC Rulebook, str. 30, *Damage Timing*

> 📖 *„If a location takes one or more points of internal structure damage, but is not outright destroyed, the attacker checks for critical damage by rolling 2D6 and consulting the Determining Critical Hits Table. On an 8 or higher, the target 'Mech takes critical damage."*
> — GoAC Rulebook, str. 30, *Critical Hits*

> 📖 *„A roll of 2 on the Hit Location Table provides a chance for a critical hit, even if the attack did not damage internal structure (though the attack must still have dealt at least 1 point of damage). This is known as a through-armor critical (TAC) hit."*
> — GoAC Rulebook, str. 31, *Through-Armor Critical Hit*

> 📖 *„Once a location has been destroyed, all further damage to that location transfers directly to the next location inward."*
> — GoAC Rulebook, str. 34, *Transferring Damage*

> 📖 *„If a location is destroyed, all components in that location are also destroyed."*
> — GoAC Rulebook, str. 34, *Destroyed Locations*
