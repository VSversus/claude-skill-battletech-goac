# Fyzické útoky (Physical Attacks) — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Making a Physical Attack (obecná pravidla) | 24–25 |
| Different Levels / Prone / Water | 25 |
| Charge Attacks | 25–26 |
| Club Attacks | 26 |
| Death From Above (DFA) | 26–28 |
| Kick Attacks | 28 |
| Physical Weapon Attacks | 28 |
| Punch Attacks | 28–29 |
| Push Attacks | 29 |
| Damage Resolution (fyzické) | 29 |

---

## Obecná pravidla

### Kdy lze fyzicky útočit
- Fyzické útoky se deklarují a rozeznávají ve **Physical Attack Phase** (fáze 4)
- Mech nesmí být prone (s výjimkou speciálních situací)
- Cíl musí být v příslušné vzdálenosti a oblouku (dle typu útoku)
- Fyzický útok **nezabrání** střelbě v témže tahu

### Base Target Number pro fyzické útoky
= **Piloting Skill** pilota (průměr IS = 5)

### Modifikátory fyzických útoků
| Situace | Modifikátor |
|---------|------------|
| Útočník šel (walked) | +0 |
| Útočník běžel (ran) | +2 |
| Útočník skočil (jumped) | +0* |
| Útočník je prone | Nelze (většina útoků) |
| Cíl je prone | Závisí na typu útoku |
| Cíl je immobilní | −4 |

*Skok je speciální případ u DFA.

### Různé výškové úrovně
- Většina fyzických útoků vyžaduje stejnou výšku
- Výjimky jsou uvedeny u jednotlivých útoků

### Prone mechs a fyzické útoky
- Obecně: prone mech **nemůže** provádět fyzické útoky
- Výjimka: viz Death from Above (DFA)

### Voda a fyzické útoky
- Depth 1 water: fyzické útoky povoleny (extra modifikátor dle typu)
- Depth 2+ water: fyzické útoky nejsou možné

## Charge Attack (nájezd/taran)

### Podmínky
- Útočník musí ukončit pohyb v hexu cíle (nebo projít skrz při překonání)
- Útočník musí **běžet** (nelze chodit ani skákat)
- Cíl nesmí být ve skoku

### Poškození útočníka
- Útočník utrpí poškození rovné **tonnage cíle ÷ 10** (zaokrouhlit nahoru)
- Hit location na útočníkovi: hod dle tabulky (přední oblouk)

### Poškození cíle
- Cíl utrpí poškození rovné **tonnage útočníka ÷ 10** (zaokrouhlit nahoru)
- Hit location na cíli: hod dle tabulky (závisí na směru)

### Displacement
- Cíl je odsunut do hexu za sebou (ve směru útoku)
- Pokud je hex obsazen: Domino Effect (viz `other-actions.md`)

### PSR
- Útočník: PSR po chargi (base +0 ze chargování, +2 za běh — platí aktuátorové modifikátory)
- Cíl: PSR po zásahu

### Hit roll
TN = Piloting Skill + modifikátory pohybu

## Club Attack (útok kmenem/tyčí)

### Podmínky
- V hexu útočníka (nebo sousedním) musí být objekt vhodný jako zbraň: zničený mech, zničená stavba, strom (Heavy Woods) nebo vhodný předmět
- Alternativa: mech bez obou paží může útočit trupem

### Poškození
- **⌊Tonnage útočníka ÷ 5⌋** (zaokrouhlit dolů)

### Hit location
- Cíl: hod na hit location (přední oblouk)

### PSR
- Útočník: PSR dle pohybu
- Cíl: PSR (base +2)

### Modifikátor útoku
- Base TN: Piloting Skill
- Cíl je na různé úrovni: nelze použít (musí být stejná výška)

## Death From Above (DFA) — "Pád shůry"

### Podmínky
- Útočník **musí skákat** a přistát v hexu cíle
- Cíl nesmí být prone

### Poškození cíle
- **⌈Tonnage útočníka ÷ 10⌉ × 3** (zaokrouhlit nahoru, pak × 3)
- Alternativní vzorec: Ceil(tonnage/10) × 3
- Příklad: 50t mech → ceil(50/10) = 5 → 5 × 3 = 15 damage

### Poškození útočníka
- Útočník utrpí **⌈Tonnage cíle ÷ 10⌉** poškození do každé nohy
- + PSR s modifikátorem (nevyhnutelný pád)

### Displacement cíle
- Cíl je odsunut z hexu (viz Displacement v `other-actions.md`)

### Útočník padá
- Útočník vždy padá po DFA (automaticky)
- PSR modifikátor: −2 (snazší PSR než standardní pád)

### Hit roll
TN = Piloting Skill + modifikátor skoku (+0 protože útočník skáče, ale special: viz níže)
- Modifikátor za skok útočníka na TN: +3 (jako standard jumping attacker modifier) MINUS odečtení za DFA specifiku? **Ne** — DFA má vlastní TN: Piloting Skill + standard jump modifiers.

## Kick Attack (kop)

### Podmínky
- Cíl musí být v **sousedním hexu** (Forward Arc nebo Side Arc)
- Útočník musí mít funkční nohu na straně, ze které kope
- Nelze, pokud útočník skákal

### Poškození
- **⌊Tonnage útočníka ÷ 5⌋** (zaokrouhlit dolů)

### Hit location
- Vždy jedna ze dvou noh cíle; hod 1D6: 1–3 = Right Leg, 4–6 = Left Leg

### Útočník: PSR
- Útočník musí provést PSR (base +0) aby sám neupadl
- Modifikátor: pokud selže crit do hip nebo nohy útočníka → +2

### PSR cíle
- Cíl: PSR (base +2)

### Omezení
- Mech s jednou nohou: nemůže kopat
- Mech v Depth 1 water: může kopat s modifikátorem +2

## Physical Weapon Attack (zbraň z torza/paže — hák, sekera atd.)

### Podmínky
- Mech musí mít fyzickou zbraň (hatchet, sword, mace atd.) instalovanou v paži nebo torzu
- *Poznámka: V GoAC základní sadě se fyzické zbraně nevyskytují; jsou v rozšířeních*

### Poškození
- Závisí na konkrétní zbrani

## Punch Attack (úder pěstí) — str. 28–29

### Podmínky
- Cíl musí být v **sousedním hexu** v **Forward Arc nebo Side Arc**
- Pokud je cíl v pravém oblouku → pouze pravá ruka; pokud vlevo → pouze levá
- Útočník **nesmí** v daném tahu střílet ze zbraní v paži, kterou pere
- Funkční **Shoulder** aktuátor v dané paži je nutný — bez něj punch nelze
- Každá ruka = samostatný hod; lze útočit jednou nebo oběma

### Poškození
- **⌈tonnage ÷ 10⌉** (zaokrouhlit **nahoru**) za každou ruku zvlášť
- Chybí nebo poškozen **Upper nebo Lower Arm Actuator**: poškození ÷ 2 (dolů), kumulativně pro každý
- Minimum poškození: 1

### TN modifikátory
| Situace | Modifikátor |
|---------|------------|
| Chybí Hand Actuator | +1 |
| Chybí Lower Arm Actuator | +2 |
| Base modifikátor punch útoku | +0 |

### Hit location
- Hod **1D6** na **Punch Location Table** (str. 28) — ne standardní Hit Location Table!

### PSR cíle
- Cíl: PSR s modifikátorem **+0**

### Speciální pravidla
- Útok oběma rukama na **dva různé cíle** je povolen — secondary target modifier se **nevztahuje**
- Pokud mech nese Physical Weapon (hatchet atd.) v paži → punch touto paží nelze

## Push Attack (strčení)

### Podmínky
- Cíl musí být v **sousedním hexu** (Forward Arc)
- Útočník musí mít funkční rameno (Shoulder) a paži

### Efekt
- Cíl je odsunut do hexu přímo za sebou (ve směru tlaku)
- Útočník se neposouvá
- Cíl: PSR (base +2); pokud selže → padá

### Poškození
- Žádné přímé poškození ze strčení samotného
- Pád způsobuje falling damage (viz `other-actions.md`)

### Podmínky selhání
- Cíl je v Depth 1 water: nelze strčit
- Hex za cílem je obsazen nebo nedostupný: Domino Effect (viz `other-actions.md`)

## Damage Resolution — fyzické útoky

Po všech fyzických útocích:
1. Aplikuj poškození na pancíř/strukturu (dle hit location)
2. Rozeznání Critical Hits (pokud IS vyčerpána)
3. PSR cíle (a útočníka dle situace)
4. Consciousness Rolls (pokud pilot utrpěl poškození)

Poškození z fyzických útoků se aplikuje **před** Heat Phase.

---

## Klíčové citace — Physical Attacks

> 📖 *„The base Target Number for a physical attack is equal to the attacking 'Mech's Piloting Skill Rating. [...] The sole exceptions are heat and sensor modifiers, which never apply."*
> — GoAC Rulebook, str. 24, *Making a Physical Attack*

> 📖 *„'Mechs can make seven different types of physical attacks: charging, clubbing, death from above (DFA), kicking, physical weapon attacks, punching, or pushing."*
> — GoAC Rulebook, str. 24, *Physical Attacks*

> 📖 *„Charge attacks are declared in the Movement Phase, not the Physical Attack Phase."*
> — GoAC Rulebook, str. 25, *Charge Attacks*

> 📖 *„A jump-capable 'Mech can leap onto its target [...]. Death from above (DFA) attacks are declared in the Movement Phase, not the Physical Attack Phase."*
> — GoAC Rulebook, str. 26, *Death From Above Attacks*

> 📖 *„A punch attack has a Damage Value of 1 for every 10 tons (or fraction of) that the attacker weighs, assigned as a single damage grouping."*
> — GoAC Rulebook, str. 28, *Punch Attacks*

> 📖 *„Kicks have a Damage Value of 1 point for every 5 tons of the attacking 'Mech's weight."*
> — GoAC Rulebook, str. 28, *Kick Attacks*
