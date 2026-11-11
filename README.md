# Monster-billede – fuld samlet filpakke (version 1.1)

Denne ZIP indeholder **alle filer i én samlet pakke**, klar til at uploades på ny til GitHub Pages.

## Filerne

- `index.html` – hele browserprototypen med HTML, CSS og JavaScript. **Monsterbilledet er indlejret i denne fil**, så det vises, selv hvis `assets`-mappen ikke er uploadet.
- `assets/` – de originale udsnit af brugerens eget monsterbillede, til eventuel senere anvendelse.
- `BILLED-PROMPT.md` – strammere billedprompt v2 til den senere AI-integration.
- `STEMME-OG-INSTRUKTION.md` – præcis tekst og funktionsbeskrivelse for monsterets velkomst.
- `README.md` – denne vejledning.

## Vigtigt om billedgenereringen

**Det grønne demo-monster er ikke AI-genereret.** Den nuværende browserapp tegner en enkel testillustration (SVG) med JavaScript ud fra nogle genkendte ord. Den kan ikke fortolke barnets fantasi på samme måde som Martin og en rigtig billedmodel. BILLED-PROMPT.md bruges derfor endnu ikke automatisk. For rigtige AI-billeder kræves en serverfunktion og en billedgenerator. Læg aldrig en API-nøgle offentligt i GitHub Pages.

## Upload alle filerne på ny til GitHub

1. Download ZIP-filen og vælg **Udpak alle**.
2. Åbn GitHub-repositoriet `Steinbeck-konsulent/monster-billede` → **Add file → Upload files**. Hvis det er tomt, brug linket **uploading an existing file**.
3. Åbn den udpakkede mappe. **Træk indholdet** (ikke selve ZIP'en eller den ydre mappe) ind på GitHub: `index.html`, markdown-filerne og gerne `assets`-mappen.
4. Tryk på **Commit changes**.
5. Under **Settings → Pages** vælg **Deploy from a branch**, `main` og `/ (root)`, hvis Pages ikke allerede er slået til.
6. Åbn `https://steinbeck-konsulent.github.io/monster-billede/` og opdatér med Ctrl+F5 ved behov.

**Kontrollér især, at `index.html` ligger i roden af repositoriet**, ikke inde i en undermappe.

## Test og privatliv

Brug din egen stemme eller testbeskrivelser, ikke børns rigtige stemmer endnu. Browserens indbyggede talegenkendelse kan sende lyd til en ekstern leverandør; at appen ikke selv gemmer lyd, er ikke det samme som at lyd behandles lokalt. Der er ingen database, login eller API-nøgle i appen. Testillustration og tekst eksisterer i browserfanen, mens den er åben; PNG gemmes kun, hvis du vælger det.
