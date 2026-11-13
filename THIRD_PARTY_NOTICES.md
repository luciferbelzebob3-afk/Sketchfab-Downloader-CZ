# Licence a oznámení třetích stran

Podklady pro **Sketchfab Downloader CZ 1.1.3**, zkontrolované **13. listopadu 2026**. Rozsah a otevřené body popisuje [LICENSING.md](LICENSING.md). Licenční texty se zachovávají v původním jazyce; český přehled je nenahrazuje.

## Původní aplikace

**skfb-glb-exporter**, autor **dlutwizard**, MIT, Copyright (c) 2026 dlutwizard.

Zdroj: [v1.1.3 / f5168793](https://github.com/dlutwizard/skfb-glb-exporter/tree/f5168793d22f9df2a4242fb863e929e67f7013ce). Přiložen je [úplný LICENSE](licenses/application/upstream-v1.1.3-LICENSE.txt), [původní oznámení](licenses/application/upstream-v1.1.3-THIRD-PARTY-NOTICES.md) a [manifest původu](licenses/application/manifest.json). Česká distribuce je úpravou tohoto projektu, nikoli tvrzením o původním autorství aplikace.

## Jádro a JavaScript

| Součást / verze | Licence či zjištěné prohlášení | Úplný text / podklady |
| --- | --- | --- |
| Sketchfab CLI engine | Místní MIT; Copyright 2026 Sketchfab CLI contributors | [LICENSE](licenses/javascript/engine-LICENSE.txt) |
| extlib | Místní MIT; Copyright 2026 anotherRandomPersonlol; zjištěn překryv s GPL projektem | [Původní oznámení](licenses/javascript/extlib-bundled-LICENSE.txt), [MIT upstreamu](licenses/javascript/extlib-declared-upstream-MIT-LICENSE.txt), [porovnání](licenses/javascript/extlib-provenance-audit.json) |
| Node.js 22.22.2 | MIT a licence zabudovaných komponent | [LICENSE s oznámeními](licenses/javascript/node-22.22.2-LICENSE.txt) |
| sharp 0.35.5 | Apache-2.0 | [LICENSE](licenses/javascript/sharp-LICENSE.txt) |
| @img/sharp-win32-x64 0.35.5 | Apache-2.0 AND LGPL-3.0-or-later | [LICENSE](licenses/javascript/sharp-win32-x64-LICENSE.txt), [závislosti](licenses/javascript/sharp-win32-x64-README.md), [verze](licenses/javascript/sharp-win32-x64-versions.json) |
| @img/colour 1.1.0 | MIT | [LICENSE](licenses/javascript/colour-LICENSE.txt) |
| detect-libc 2.1.2 | Apache-2.0 | [LICENSE](licenses/javascript/detect-libc-LICENSE.txt) |
| semver 7.8.5 | ISC | [LICENSE](licenses/javascript/semver-LICENSE.txt) |

MIT prohlášení extlib není tímto přehledem potvrzeno jako jediné možné licenční zařazení. Uchována je i [GPL licence porovnávaného projektu](licenses/javascript/extlib-matching-upstream-GPL-3.0.txt). Důkazy a omezení jsou uvedeny v porovnání původu; místní licence nebyly přepsány ani odstraněny.

## Python balíčky uvnitř EXE

| Balíček / verze | Licence | Úplné texty |
| --- | --- | --- |
| certifi 2026.10.23 | MPL-2.0 | [Oznámení Mozilla / ca-bundle](licenses/python-packages/certifi/LICENSE), [MPL 2.0](licenses/python-packages/certifi/MPL-2.0.txt) |
| charset-normalizer 3.5.2 | MIT | [LICENSE](licenses/python-packages/charset-normalizer/LICENSE) |
| idna 3.20 | BSD-3-Clause | [LICENSE](licenses/python-packages/idna/LICENSE.md) |
| requests 2.34.2 | Apache-2.0 | [LICENSE](licenses/python-packages/requests/LICENSE), [NOTICE](licenses/python-packages/requests/NOTICE) |
| urllib3 2.8.0 | MIT | [LICENSE](licenses/python-packages/urllib3/LICENSE.txt) |

[Manifest](licenses/python-packages/manifest.json) uvádí přesná oficiální vydání PyPI, SHA-256 a zdrojové archivy. Tyto archivy nejsou automaticky zdroji případných místních úprav.

## Python a nativní runtime

| Součást / verze | Podmínky | Úplné texty |
| --- | --- | --- |
| CPython 3.11.5 | PSF a historické / převzaté licence | [LICENSE](licenses/runtime/python-3.11.5-LICENSE.txt), [začleněné součásti](licenses/runtime/python-3.11.5-incorporated-licenses.rst) |
| PyInstaller 6.10.0 | GPL-2.0-or-later s výjimkou pro bootloader; další části dle COPYING | [COPYING včetně výjimky](licenses/runtime/pyinstaller-6.10.0-COPYING.txt) |
| Tcl 8.6.12 | Tcl licence | [license.terms](licenses/runtime/tcl-8.6.12-license.terms) |
| Tk 8.6.12 | Tk licence | [license.terms z balíčku](licenses/runtime/tk-8.6.12-license.terms) |
| OpenSSL 3.5.7 | Apache-2.0 | [LICENSE](licenses/runtime/openssl-3.5.7-LICENSE.txt) |
| zlib 1.2.13 | zlib | [README s copyrightem a licencí](licenses/runtime/zlib-1.2.13-README.txt) |
| liblzma / XZ Utils 5.4.2 | liblzma deklarována jako public domain; další části zvlášť | [COPYING](licenses/runtime/xz-5.4.2-COPYING.txt) |
| Expat 2.5.0 v pyexpat | MIT | [COPYING](licenses/runtime/expat-2.5.0-COPYING.txt) |
| bzip2 1.0.8 | bzip2 licence | [LICENSE](licenses/runtime/bzip2-1.0.8-LICENSE.txt) |

[Inventář binárních souborů](licenses/runtime/binary-inventory.json) zaznamenává verze a hashe samostatných runtime DLL i obou místních EXE. `SketchfabTest.exe` je pouze inventarizován. U `ffi.dll` a Microsoft DLL zbývají podklady uvedené v [LICENSING.md](LICENSING.md).

## Obrazové knihovny sharp/libvips

Balíček deklaruje libvips 8.18.7 a další knihovny pod MIT, BSD, Apache, LGPL, MPL a jinými podmínkami. [Strojově čitelný inventář](licenses/javascript/sharp-native-components.json) vychází z místního seznamu verzí a licencí. Verze stejnojmenných knihoven této skupiny se mohou lišit od Python runtime.

Přiloženy jsou [licence vydání libvips](licenses/javascript/libvips-win64-8.18.7-LICENSE.txt) a referenční texty [GPL 3](licenses/javascript/GPL-3.0.txt), [LGPL 3](licenses/javascript/LGPL-3.0.txt) a [MPL 1.1](licenses/javascript/MPL-1.1.txt). Samy netvoří úplná autorská oznámení všech transitivních knihoven ani nabídku odpovídajících zdrojů. Neověřené položky jsou vyznačeny v inventáři.

## Modely a textury

Repozitář neobsahuje modely ani textury ze Sketchfabu. Jejich práva náleží příslušným autorům; licence aplikace nezakládá oprávnění k jejich dalšímu použití. Projekt není oficiálním produktem Sketchfab či Epic Games.
