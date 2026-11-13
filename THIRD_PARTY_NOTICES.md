# Původ a licence komponent

Tento dokument zaznamenává licenční údaje nalezené v místním balíčku **Sketchfab Downloader CZ 1.1.3** se sestavením ze dne **3. listopadu 2026**. Popsané komponenty ani spustitelné soubory aplikace nejsou součástí tohoto repozitáře.

Jde o přehled dostupných podkladů, **nikoli o úplný soubor licenčních oznámení pro distribuci aplikace**. Cesty níže označují soubory v místním balíčku, nikoli soubory zveřejněné v tomto repozitáři.

## Zjištěné licenční údaje

| Komponenta | Zdroj údaje v balíčku | Zjištěné označení |
| --- | --- | --- |
| Stahovací jádro | `_internal/engine/LICENSE` | MIT; Copyright (c) 2026 Sketchfab CLI contributors |
| JavaScriptové moduly `extlib` | `_internal/extlib/LICENSE` | MIT; Copyright (c) 2026 anotherRandomPersonlol |
| `sharp` | `_internal/node_modules/sharp/package.json` | Apache-2.0 |
| `@img/sharp-win32-x64` | `_internal/node_modules/@img/sharp-win32-x64/package.json` | Apache-2.0 AND LGPL-3.0-or-later |

## Původ modulů extlib

Soubor `_internal/extlib/LICENSE` uvádí jako původ projektu [anotherRandomPersonlol/Sketchfab-Ripper](https://github.com/anotherRandomPersonlol/Sketchfab-Ripper). Podle tohoto místního oznámení byly části původního userscriptu `src/Sketchfab-ripper.user.js` rozděleny do 18 modulů ES pro použití v prostředí Node.js. Uvedená licence a autorská atribuce patří původnímu autorovi.

Odkaz a popis původu jsou převzaty z licenčního oznámení přiloženého k balíčku; tento přehled nepotvrzuje aktuální obsah odkazovaného repozitáře ani shodu jednotlivých verzí.

## Rozsah dostupných podkladů

Balíček dále obsahuje běhové prostředí Pythonu a Node.js, Tcl/Tk a další knihovny. Výše uvedená tabulka není úplným inventářem všech závislostí a jejich licenčních podmínek.

Přiložený `_internal/CHANGELOG.md` uvádí u verze 1.1.3 přidání kořenového souboru `LICENSE` s licencí MIT a souboru `THIRD-PARTY-NOTICES.md`. Tyto dva soubory ale v prohlédnutém místním balíčku nebyly nalezeny. Úplné zdroje grafického rozhraní a sestavovací skripty podle dodaného návodu rovněž nejsou jeho součástí.

Z těchto podkladů proto tento repozitář neodvozuje ani neuděluje novou licenci pro celý binární balíček. Případné budoucí zveřejnění aplikace musí mít vlastní odpovídající licenční dokumentaci a zachovat příslušná oznámení jednotlivých komponent.

## Licence tohoto repozitáře

[MIT licence tohoto repozitáře](LICENSE) se týká pouze jeho nově vytvořené dokumentace. Nijak nepřelicencovává aplikaci, komponenty třetích stran ani modely a textury. Práva k nim zůstávají jejich příslušným autorům a držitelům práv.
