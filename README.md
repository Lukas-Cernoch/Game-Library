# 🎮 Game List

Cross-platform aplikace napsaná v **Angularu** a **Ionic Frameworku** (s **Capacitorem** pro nativní mobilní build), která přes **RAWG API** stahuje katalog her a umožňuje uživateli vybrat si oblíbené tituly na přehlednou hlavní obrazovku, kde si u každé hry může zobrazit podrobné informace. Díky Ionic/Capacitoru lze aplikaci spustit jako web i zabalit jako nativní Android/iOS aplikaci ze stejného zdrojového kódu.

## ✨ Funkce

- **Výběr her ze seznamu** — modální okno se scrollovatelným seznamem her a zaškrtávacími políčky
- **Přizpůsobitelná hlavní obrazovka** — vybrané hry se zobrazí jako dlaždice s obrázkem a hodnocením
- **Detail hry** — obrázek, popis, doba hraní (Play Time), datum vydání (Release Date), hodnocení (Rating), platformy a systémové požadavky (PC Requirements)
- **Data z veřejného API** — hry, hodnocení a popisy stahovány dynamicky přes RAWG API
- **Cross-platform** — jedna codebase pro web i nativní mobilní aplikaci (Capacitor)

## 🖥️ Ukázka aplikace

**Výběr her ze seznamu**
![Výběr her](gamelist-screenshots/vyber-her.png)

**Hlavní obrazovka s vybranými hrami**
![Hlavní obrazovka](gamelist-screenshots/hlavni-obrazovka.png)

**Detail hry**
![Detail hry](gamelist-screenshots/detail-hry.png)

## 🛠️ Použité technologie

| Technologie | Účel |
|---|---|
| Angular / TypeScript | frontend framework a hlavní jazyk aplikace |
| Ionic Framework | UI komponenty a cross-platform vrstva |
| Capacitor | zabalení aplikace do nativního Android/iOS buildu |
| RxJS | práce s asynchronními daty (HTTP volání) |
| RAWG API | zdroj dat o hrách — hodnocení, popisy, platformy, obrázky |

## 🚀 Spuštění projektu

### Požadavky
- Node.js a npm
- Angular CLI / Ionic CLI
- Vlastní API klíč z [rawg.io](https://rawg.io/apidocs)

### Postup — spuštění ve webu
1. Naklonujte repozitář:
   ```bash
   git clone <ODKAZ_NA_REPO>
   ```
2. Nainstalujte závislosti:
   ```bash
   npm install
   ```
3. Do `src/services/games/games.service.ts` doplňte vlastní RAWG API klíč do proměnné `apiKey` (klíč není součástí repozitáře z bezpečnostních důvodů).
4. Spusťte vývojový server:
   ```bash
   ionic serve
   ```
5. Otevřete `http://localhost:4200` v prohlížeči.

### Postup — mobilní build (Android)
```bash
ionic build
npx cap sync android
npx cap open android
```
Aplikace se otevře v Android Studiu, odkud ji lze spustit na emulátoru nebo fyzickém zařízení.

## 👤 Autor

**Lukáš Černoch**
[GitHub](https://github.com/Lukas-Cernoch)

