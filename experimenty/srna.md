---
description: Systém Rychlého NAsycení (SRNA)
---

# SRNA

Nasycený návštěvník je spokojený návštěvník - ale klasické systémy cateringu selhávají a mají své výrazné omezení (viz. tabulka níže). Náš lehce škálovatelný a flexibilní systém SRNA má ambice většinu těchto omezení eliminovat, za pomoci moderních technologií a jednoho jediného kompromisu - jídlo je nutné si objednat předem (minimálně cca 2-3h).

### Srovnání přístupu ke cateringu

| Typ                   | Výhody                                                                                                                                                                                                  | Nevýhody                                                                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| **Klasický catering** | <ul><li>bez starostí - catering firma vše zařídí</li><li>lze umístit uvnitř</li><li>rychlé pro návštěvníka</li></ul>                                                                                    | <ul><li>mizerný výběr jídel</li><li>omezené použití pro akce, která nemají jídlo v ceně </li></ul>                                       |
| **Food-trucky**       | <ul><li>vhodné pro akce bez jídla v ceně vstupenky</li><li>relativně bezstarostné</li></ul>                                                                                                             | <ul><li>nízká kapacita (fronty)</li><li>velká vzdálenost pro návštěvníky</li><li>nutnost ručení tržeb</li><li>vázané na počasí</li></ul> |
| **SRNA**              | <ul><li>výborný výběr</li><li>velká kapacita - lehce škálovatelné</li><li>blízko návštěvníkovi</li><li>podpora místních podniků</li><li>pro zodpovědného návštěvníka minimálně časově náročné</li></ul> | <ul><li>jídlo není hned - u návštěvníka do 2-3h</li><li>vyžaduje objednávkový systém a SRNA tým (zatím nejde outsourcovat)</li></ul>     |

## Objednávkový systém

### Terminologie

* **časový blok** (50 minut) - ucelený doručovací blok, např. oběd, večeře
* **časový slot** (5 minut) - upřesňující segment v rámci časového bloku, každý blok má 10 slotů
* [**výdejní místo**](srna.md#vydejni-mista) - konkrétní místo, kde si návštěvník objednávku vyzvedne

### Číslování objednávek

Každá objednávka bude mít svůj unikátní kód, ze kterého půjde lehce vydedukovat časový blok a výdejní místo, na které směřuje.

#### Ukázkový příklad: `A123`

| Znaky | Význam          | Možnosti |
| ----- | --------------- | -------- |
| `A`   | výdejní místo   | `A-Z`    |
| `1`   | časový blok     | `1-9`    |
| `2`   | časový slot     | `0-9`    |
| `3`   | pořadí ve slotu | `0-9`    |

## Centrální logistický uzel

Centrální logistický uzel je místo v rámci místa konání konference, kam se jídla z restaurací a dalších podniků (objednávky) fyzicky přiváží a odkud jsou posléze distribuovány na jednotlivá [vydejní místa](srna.md#odberove-mista).

### Naskladnění objednávek

Při příjmu se každá jednotlivá objednávka naskenuje do systému a fyzicky rozřadí podle výdejního místa na které směruje.

### Vyskladnění objednávek - distribuce na výdejní místa

Součástí týmu centrálního logistického uzlu budou lidé, kteří budou za pomoci vozíků vozit objednávky z centrálního uzlu do výdejních míst.

## Výdejní místa

Na výdejním místě si návštěvníci svoje objednávky vyzvedávají a neslouží k jinému dalšímu účelu.

### Součásti výdejního místa

* Obsluha - minimálně 1 člověk
* Telefon + SRNA aplikace - na skenování QR kódů
* LCD Obrazovka + RPi - informační systém o stavu objednávek pro návštěvníky

### Proces vyzvednutí objedávky

Celý proces by měl trvat zhruba 30 sekund.

1. Návštěvník příjde a ukáže svoji konferenční visačku s QR kódem
2. Obsluha naskenuje QR kód pomocí aplikace v telefonu (15s)
3. Aplikace v telefonu ukáže zda je objednávka přítomná, její kód, případně kde ji hledat
4. Obsluha objednávku najde a předá návštěvníkovi (15s) - hotovo&#x20;



