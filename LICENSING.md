# Licenční podklady české distribuce

Stav k **13. listopadu 2026**, místní balíček **1.1.3**.

## Původ aplikace

Česká distribuce vychází z projektu [dlutwizard/skfb-glb-exporter](https://github.com/dlutwizard/skfb-glb-exporter), který jako zdroj označil správce této distribuce. Ověřen byl tag **v1.1.3**, commit [f5168793d22f9df2a4242fb863e929e67f7013ce](https://github.com/dlutwizard/skfb-glb-exporter/tree/f5168793d22f9df2a4242fb863e929e67f7013ce).

Původní autor **dlutwizard** poskytuje vlastní projekt pod licencí **MIT**. Její [úplný původní text](licenses/application/upstream-v1.1.3-LICENSE.txt) je zachován beze změny, včetně copyrightu **Copyright (c) 2026 dlutwizard**. Přiložena jsou i [původní oznámení verze 1.1.3](licenses/application/upstream-v1.1.3-THIRD-PARTY-NOTICES.md).

Z 25 porovnaných souborů jádra, modulů extlib a jejich licencí je 18 bajtově shodných s uvedeným tagem. [Manifest původu](licenses/application/manifest.json) uvádí jednotlivé výsledky. Český EXE není tímto označen za reprodukovatelné sestavení původních zdrojů; úplné zdroje českých úprav nejsou v tomto repozitáři.

## Rozsah licencí

- Kořenový [LICENSE](LICENSE) pokrývá původní dokumentaci tohoto repozitáře.
- Původní aplikace má samostatnou MIT licenci autora dlutwizard uvedenou výše.
- Kopie licencí a oznámení ve složce `licenses/` zůstávají pod původními podmínkami a se zachovanou atribucí. Některé obecné texty jsou přiloženy pro referenci; jejich přítomnost sama neuděluje licenci ke konkrétnímu souboru.
- Licence programu se nevztahují na stažené modely a textury ani na značky Sketchfab či Epic Games.

## Obsah podkladů

[Český přehled komponent](THIRD_PARTY_NOTICES.md) odkazuje na úplné licenční texty a oznámení. Manifesty ve skupinách [application](licenses/application/manifest.json), [python-packages](licenses/python-packages/manifest.json), [runtime](licenses/runtime/manifest.json) a [javascript](licenses/javascript/manifest.json) obsahují zdroje, verze a SHA-256.

Texty pocházejí z místního balíčku nebo odpovídajících vydání upstream projektů. Python balíčky byly identifikovány statickým čtením archivu EXE. Aplikace ani kód balíčků nebyly při kontrole spuštěny. Licenční texty jsou zachovány v původním jazyce; český přehled je nenahrazuje.

## Otevřené body distribuce celého balíčku

1. **Překryv původu extlib a WASM.** Místní i původní oznámení aplikace deklarují MIT. Čtrnáct souborů extlib a soubor WASM jsou současně bajtově shodné se soubory jiného projektu zveřejněného pod GPL-3.0. [Porovnání](licenses/javascript/extlib-provenance-audit.json) uchovává konkrétní verze a hashe. Shoda sama neprokazuje pořadí autorství ani nevylučuje samostatné či duální MIT oprávnění. Pro jednoznačné zařazení je třeba doložit oprávnění k těmto souborům, případně splnit podmínky příslušné GPL distribuce. Není tím řečeno, že celý program musí automaticky změnit licenci na GPL.
2. **Nativní knihovny sharp/libvips.** Obsahují také LGPL a MPL komponenty. Obecný text licence nenahrazuje autorská oznámení jednotlivých knihoven, odpovídající zdroje a případné podklady k úpravě či opětovnému propojení. [Inventář](licenses/javascript/sharp-native-components.json) označuje neověřené položky. Samotná existence DLL nepotvrzuje splnění všech podmínek.
3. **Samostatná ffi.dll a Microsoft runtime.** Verze `ffi.dll` nebyla určena. U `VCRUNTIME140.dll`, `ucrtbase.dll` a `api-ms-win-*.dll` jsou zaznamenány verze a hashe, ale původní instalační či sestavovací podklady k redistribuci nebyly přiloženy. Relevantní podmínky popisuje [Microsoft](https://learn.microsoft.com/en-us/cpp/windows/redistributing-visual-cpp-files?view=msvc-170).

Původní licence hlavní aplikace je nyní doložena. Tento přehled neprohlašuje zbývající podmínky pro distribuci celého binárního balíčku za vyřešené a nepřelicencovává cizí komponenty.
