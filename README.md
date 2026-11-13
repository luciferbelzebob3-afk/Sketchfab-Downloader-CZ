# Sketchfab Downloader CZ

![Windows](https://img.shields.io/badge/platform-Windows-0078D4)
![Čeština](https://img.shields.io/badge/jazyk-%C4%8De%C5%A1tina-D7141A)
![GLB](https://img.shields.io/badge/export-GLB-4C9A2A)

**České rozhraní nástroje pro stahování modelů ze Sketchfabu a export do GLB s materiály a texturami.** Přenosný balíček pro Windows nabízí dávkové zpracování odkazů, přehled průběhu a ovládání z příkazové řádky.

Česká distribuce vychází z projektu [dlutwizard/skfb-glb-exporter](https://github.com/dlutwizard/skfb-glb-exporter), jehož autorem je **dlutwizard**. Tento repozitář představuje českou verzi a shromažďuje její dokumentaci. Jde o nezávislý, neoficiální projekt bez spojení se společností Sketchfab.

## Stav zveřejnění

| Položka | Stav |
| --- | --- |
| Dokumentovaný místní balíček | Verze **1.1.3**, sestavení **3. listopadu 2026** |
| Obsah tohoto repozitáře | Dokumentace a informace o licencích |
| Instalační nebo přenosný archiv | Zatím není zveřejněn |
| Úplné zdrojové soubory aplikace | Zatím nejsou zveřejněny |

Popis funkcí vychází z návodu a metadat uvedeného balíčku. Aktuální funkčnost vůči službě Sketchfab zde nebyla ověřena.

## Co aplikace nabízí

- **České grafické rozhraní** s ukazatelem průběhu a protokolem jednotlivých úloh.
- **Dávkové zpracování** více modelů; každý odkaz se zadává na samostatný řádek.
- Podporu plných adres modelů, zkrácených odkazů `skfb.ly` a 32znakových ID modelů.
- Odstranění duplicitních odkazů podle ID modelu a nastavení **1–5 souběžných úloh**.
- **Export GLB s vloženými materiály a texturami** pro další práci například v Blenderu.
- Zobrazení informací o modelu, jeho licenci a dostupnosti oficiálního stažení.
- Příkazovou řádku, diagnostiku prostředí a přenosný režim nastavení.

## Použití již získaného balíčku

Tento postup je určen uživatelům, kteří už mají celý balíček aplikace. Samotné stažení tohoto repozitáře aplikaci neposkytuje.

1. Rozbalte celý balíček do vlastní složky ve Windows.
2. Spusťte `Sketchfab Stahovač.exe`.
3. Vložte odkazy do pole **Odkazy na modely**, každý na samostatný řádek.
4. Vyberte výstupní složku a požadovaný počet souběžných úloh.
5. Klikněte na **Spustit stahování** a sledujte průběh v protokolu.
6. Přes **Otevřít výstupní složku** přejděte k výsledkům.

**Složka `_internal` musí zůstat vedle souboru EXE.** Podle přiloženého návodu si balíček nese potřebné běhové knihovny; samostatná instalace Pythonu ani Node.js není nutná. Pro získávání modelů potřebuje připojení k internetu.

Hlavním výsledkem je soubor `<název modelu>_full.glb`. V Blenderu jej otevřete přes **File → Import → glTF 2.0**. Materiály zobrazíte v režimu **Material Preview**.

### Příkazová řádka

V PowerShellu otevřeném ve složce aplikace lze použít například:

```powershell
& '.\Sketchfab Stahovač.exe' --version
& '.\Sketchfab Stahovač.exe' --env
& '.\Sketchfab Stahovač.exe' --run 'ODKAZ_NA_MODEL' --out 'D:\Modely' --conc 3
```

Zástupný text `ODKAZ_NA_MODEL` nahraďte skutečným odkazem. Přepínač `--conc` nastavuje souběžnost v rozsahu 1–5; `--portable` vynutí ukládání nastavení do složky programu. Podrobnosti obsahuje návod dodaný s balíčkem.

## Licence a původ

Původní aplikace **skfb-glb-exporter** je zveřejněna pod **MIT**, Copyright (c) 2026 **dlutwizard**. [Původní licence verze 1.1.3](licenses/application/upstream-v1.1.3-LICENSE.txt) byla obnovena beze změny.

[MIT licence tohoto repozitáře](LICENSE) se vztahuje na nově vytvořenou dokumentaci. Kopie cizích licencí a oznámení, aplikace a její závislosti mají své vlastní podmínky. Podrobnosti, zdroje a zbývající otázky distribuce obsahují [licenční podklady](LICENSING.md) a [přehled komponent](THIRD_PARTY_NOTICES.md).

Licence programu se nevztahuje na modely a textury třetích stran. Používejte jen obsah, k jehož stažení a zamýšlenému použití máte oprávnění.

## Chyby, nápady a podpora projektu

Návrhy na zlepšení překladu, dokumentace nebo aplikace můžete přidat do [GitHub Issues](https://github.com/luciferbelzebob3-afk/Sketchfab-Downloader-CZ/issues). U chyby uveďte verzi aplikace, verzi Windows, postup reprodukce a relevantní část protokolu bez osobních údajů či přihlašovacích údajů.

Pokud vám projekt pomáhá, můžete jej podpořit hvězdičkou na GitHubu nebo sdílením odkazu na tento repozitář.

## English summary

**Sketchfab Downloader CZ** documents a Czech-language portable Windows application for batch Sketchfab model downloads and GLB export with materials and textures. The documented local package is version **1.1.3**, built on **November 3, 2026**.

This repository currently contains **documentation only**. No application archive or complete application source code is published here. The original application by **dlutwizard** is MIT-licensed; its original license is preserved in this repository. The repository-level MIT license covers original documentation only. Third-party components and reproduced notices retain their own terms; see [licensing details](LICENSING.md) for the recorded evidence and unresolved distribution questions. This is an independent, unofficial project; use only content you are authorized to download and use.
