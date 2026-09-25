# Koartje releases

Hier staan de installers en updatebestanden van Koartje, een roadmaptool bovenop Azure DevOps. De broncode staat in een aparte, besloten repository.

## Downloaden

Kies onder [Releases](https://github.com/joepvanabeelen/koartje-releases/releases/latest) het bestand voor jouw computer:

- **Windows, installer** (`Koartje-Setup-<versie>.exe`): installeert per gebruiker in je eigen profiel, zonder beheerdersrechten, en werkt zichzelf automatisch bij.
- **Windows, portable** (`Koartje-<versie>-portable-x64.exe` of `-arm64.exe`): niets installeren, direct starten. Meldt nieuwe versies, maar werkt zichzelf niet bij.
- **Windows, zip** (`Koartje-<versie>-win-x64.zip` of `-arm64.zip`): uitpakken en `Koartje.exe` starten. Meldt nieuwe versies.
- **macOS** (`Koartje-<versie>-arm64.dmg` voor Apple Silicon, `Koartje-<versie>.dmg` voor Intel). Meldt nieuwe versies.

De builds zijn niet ondertekend. Windows kan daarom "Windows heeft uw pc beschermd" tonen (kies *Meer info → Toch uitvoeren*), en macOS vraagt de eerste keer om de app via rechtsklik → *Open* te starten.

## Voor de updater

De app leest `latest.yml` (Windows) uit de nieuwste release en controleert elke download met de SHA-512-hash daarin. Verwijder deze bestanden niet uit een release.
