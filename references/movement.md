# Pohyb (Movement) — GoAC

## Čísla stránek (GoAC Rulebook)
| Sekce | Strana |
|-------|--------|
| Movement Modes (Standing/Walking/Running/Jumping) | 8 |
| Movement Basics (Facing, Ground Movement) | 9 |
| Terrain / Movement Costs Table | 9–10 |
| Minimum Movement | 11 |
| Immobile | 11 |
| Stacking | 11 |
| Jumping Movement | 11 |
| Prone BattleMechs | 12 |
| Movement in Water | 12 |

---

## Pohybové módy

| Mód | Útočník modif. | Cíl modif. | Heat | Poznámky |
|-----|---------------|-----------|------|---------|
| Stojí (Standing Still) | +0 | +0 | 0 | Nesmí utrácet MP, ani měnit orientaci |
| Chůze (Walking) | +1 | Dle hexů | 1 | Může chodit pozpátku |
| Běh (Running) | +2 | Dle hexů | 2 | Nesmí pozpátku; Run MP = Walk MP × 1,5 (zaokrouhlit nahoru) |
| Skok (Jumping) | +3 | +1 + dle hexů | 1/hex (min. 3) | Musí stát na začátku tahu; ignoruje terénní PSR |

**Cílový modifikátor "dle hexů"** — viz tabulka v `tables.md` (Attack Modifiers Table).

## Základy pohybu

### Orientace (Facing)
- Každý hex má 6 stran (hexsides); mech musí vždy čelit jedné z nich
- Mech se orientuje směrem, kam míří jeho nohy
- Změna orientace = 1 MP za každý hexside (180° = 3 MP)
- Torso twist **nemění** orientaci, pouze palebné oblouky

### Pohyb vpřed/vzad
- Vpřed: do hexu před mechem
- Vzad: do hexu přímo za mechem (pouze chůze, nikoli běh; nesmí měnit úrovně)
- Pohyb do jiného hexu vyžaduje nejprve změnu orientace

### Úrovně (Level Change)
- Pohyb vpřed: lze změnit úroveň max. o 1–2 levely za hex (+1 MP/level, nahoru i dolů)
- Pohyb vzad: nelze měnit úrovně
- Nucená změna: nelze vynutit vstup do hexu 3+ levelů výše; dolů lze libovolně (2+ levely dolů = automatický pád)

### Obsazené hexy
- Přes hex s přátelským mechem lze projít
- Hex s nepřátelským mechem nelze přejít (pouze charge útok)
- Mech **nesmí skončit** pohyb ve stejném hexu jako jiný mech

### Stacking
- Na konci pohybové fáze: max. 1 mech na hex
- Porušení = Displacement (viz `other-actions.md`)

## Terén

### Movement Costs Table

| Terén / Akce | MP cena | PSR? |
|-------------|---------|------|
| Vstup do libovolného hexu (základ) | 1 | — |
| Clear | +0 | — |
| Paved/Bridge | +0 | — |
| Road (podél) | +0* | — |
| Rough | +1 | — |
| Light Woods | +1 | — |
| Heavy Woods | +2 | — |
| Water Depth 1 | +1** | Ano (−1) |
| Water Depth 2+ | +3** | Ano (+0, Depth 3+: +1) |
| Level change 1 | +1 | — |
| Level change 2 | +2 | — |
| Rubble | +1 | Ano (+0) |
| Změna orientace | 1/hexside | — |
| Lehnout (Dropping) | 1 | — |
| Vstát (Standing Up) | 2/pokus | Ano (+0) |

*Jede-li mech podél cesty; jinak cena podkladového terénu.
**MP cena za pohyb po dně vodního hexu (nezahrnuje MP za změnu úrovně).

### Typy terénu pro LOS
- **Clear**: bez modifikací
- **Light Woods**: 3 intervening hexy blokují LOS
- **Heavy Woods**: 1× Light + 1× Heavy blokují LOS (nebo 2× Heavy)
- **Water Depth 1+**: viz `combat.md` pro LOS pravidla
- **Rough/Rubble**: neblokuje LOS

## Minimum Movement
Mech se může posunout do hexu přímo před sebou, i kdyby normálně neměl dost MP, pokud:
- Má alespoň 1 MP
- Vstup do hexu není zakázán (Level Change)
- Toto je jeho **jediný** pohyb (žádná změna orientace atd.)
- Pohyb se počítá jako **běh**

## Immobilní mech
Nelze pohybovat žádným způsobem.
- Útok na immobilní cíl: −4 TN modifikátor
- Immobilní: shutdown, opuštěný, bez všech 4 končetin, pilot v bezvědomí
- **Není** immobilní: stojící mech, prone mech, mech s 0 MP z aktuátorů/heat, mech s vyřazeným gyrem

## Skok (Jumping Movement)
- Musí stát na začátku tahu (ne prone)
- 1 MP = 1 hex bez ohledu na terén (pokud je legální vstoupit)
- Mech může skočit do stejného hexu, kde začal (za 1 MP)
- Přeskakuje mchy a terén bez PSR za průchod
- Orientace po přistání je libovolná (zadarmo)
- Výpočet výšky skoku: Jumping MP + level startovního hexu musí ≥ level překonávaného terénu
- Z vody: jump jety v ponořených nohách **nelze použít**

### Kritické poškození a skok
Každý z těchto kritů vyžaduje PSR při přistání:
- Ztráta nohy, crit do gyra, crit do boků (hip), crit do jakéhokoliv aktuátoru nohy

## Prone BattleMechs

### Lehnutí (Dropping to Ground)
- Cena: 1 MP
- Lze kdykoliv v pohybové fázi

### Pohyb v prone
- Lze pouze měnit orientaci v hexu nebo vstát
- Nelze skákat

### Vstávání (Standing Up)
- Cena: 2 MP za pokus (úspěšný i neúspěšný)
- PSR (base +0)
- Při neúspěchu: mech padá znovu + falling damage + možné poškození pilota
- Lze opakovat, dokud zbývají MP
- Po úspěšném vstání: libovolná orientace (zadarmo)
- Heat: 1 bod za každý pokus
- Chybí obě nohy nebo (1 noha + obě paže): **nelze vstát**
- 1 noha: max. 1 pokus za tah, vždy jako running

## Pohyb ve vodě
- Vstup do vody Depth 1+: PSR
- Nesmí vstoupit do Depth 1+ water při **běhu** (lze měnit orientaci nebo odejít z vody)
- Depth 1 water: mech je ponořen po pás (levely fungují jako záporné)
- Depth 2+ water: hluboká voda — zvláštní pravidla viz `combat.md` a `damage.md`

---

## Klíčové citace — Movement

> 📖 *„Every 'Mech must be assigned one (and only one) of the movement modes available to it."*
> — GoAC Rulebook, str. 8, *Movement Modes*

> 📖 *„A 'Mech's Running MP rating is equal to its Walking MP times 1.5, rounding up."*
> — GoAC Rulebook, str. 8, *Running*

> 📖 *„Using jump jets always generates a minimum of 3 heat points, no matter how far a 'Mech jumps."*
> — GoAC Rulebook, str. 8, *Jumping*

> 📖 *„A 'Mech can move forward into the hex it is facing, or backward into the hex directly to its rear. It cannot move into any other hex without first changing its facing."*
> — GoAC Rulebook, str. 9, *Ground Movement*

> 📖 *„When moving forward a 'Mech may change levels (or depths) by only 1 or 2 levels per hex, at an additional cost of 1 MP per level (whether up or down)."*
> — GoAC Rulebook, str. 9, *Level Change*

> 📖 *„An immobile 'Mech cannot make movements of any kind. Attacks against an immobile target apply a –4 Target Number modifier."*
> — GoAC Rulebook, str. 11, *Immobile*

> 📖 *„A 'Mech can move into the hex directly in front of it, even if it does not have the MP normally required [...]. To enter a hex in this fashion, a 'Mech must use running movement."*
> — GoAC Rulebook, str. 11, *Minimum Movement*

> 📖 *„'Mechs cannot enter a Depth 1 or deeper water hex while running."*
> — GoAC Rulebook, str. 8, *Running* (Water)
