# BeKeto Studio — pobieranie i aktualizacje

Aplikacja do generowania grafik marketingowych BeKeto (Windows + macOS).
To repozytorium zawiera **wyłącznie gotowe instalki** — kod źródłowy jest prywatny.

## ⬇️ Pobierz najnowszą wersję
➡️ **[Najnowsze wydanie (Releases)](https://github.com/BeKetoSpecialist/beketo-studio-app-live/releases/latest)**

Pobierz **jeden** plik pod swój system:

| System | Plik |
|---|---|
| **Windows** | `BeKeto-Studio-Setup-X.Y.Z.exe` |
| **Mac — Apple M1/M2/M3/M4** | `BeKeto-Studio-X.Y.Z-arm64.dmg` |
| **Mac — Intel (starszy)** | `BeKeto-Studio-X.Y.Z-x64.dmg` |

> Jak sprawdzić Maca: menu Apple  → „O tym Macu". „Chip Apple M…" = wersja **arm64**; „Procesor Intel" = **x64**.
> Plików `.blockmap` i `.yml` nie pobierasz — służą do automatycznych aktualizacji.

## Pierwsza instalacja
Program jest niepodpisany (wewnętrzny, bez płatnego certyfikatu Apple/Microsoft), więc system raz pokaże ostrzeżenie:

**Windows:** „Więcej informacji" → „Uruchom mimo to".

**Mac — pierwsza instalacja (jednorazowo na komputer):**
1. Otwórz pobrany `.dmg` i przeciągnij **BeKeto Studio** do **Applications** (Programy).
2. Otwórz **Terminal** (Launchpad → wpisz „Terminal"), wklej i zatwierdź Enterem:
   ```
   xattr -cr "/Applications/BeKeto Studio.app"
   ```
3. Uruchom BeKeto Studio normalnie (dwuklik). Gotowe.

> Skąd ta komenda? Aplikacja jest niepodpisana (nie płacimy Apple $99/rok za certyfikat dla
> narzędzia wewnętrznego), a Safari oznacza każdy pobrany plik flagą kwarantanny — macOS
> pokazuje wtedy mylący błąd „Rzecz jest uszkodzona". Komenda zdejmuje flagę; plik jest cały.
> Na nowszych macOS (15+) sztuczki „prawy przycisk → Otwórz" już nie działają, więc Terminal
> to najpewniejsza droga. **Od wersji 0.2.8 robisz to tylko RAZ** — kolejne aktualizacje
> aplikacja pobiera i instaluje sama (patrz niżej).

## Aktualizacje — automatyczne (Windows i Mac)
Program sam sprawdza i pobiera nowe wersje przy uruchomieniu — wystarczy normalnie korzystać
z aplikacji i kliknąć „Uruchom ponownie teraz", gdy pojawi się baner.

> Mac: automatyczne aktualizacje działają od wersji **0.2.8** (aplikacja pobiera je sama,
> więc macOS nie nakłada kwarantanny). Jeśli masz starszą wersję — zrób raz „pierwszą
> instalację" wg instrukcji wyżej. Gdyby automatyczna aktualizacja kiedyś się nie powiodła
> (np. brak uprawnień do Programów), aplikacja pokaże baner z linkiem do ręcznego pobrania.
