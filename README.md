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

**Mac (od wersji 0.2.3):**
1. Otwórz pobrany `.dmg` (dwuklik).
2. W oknie, które się otworzy, kliknij **prawym przyciskiem** na `Zainstaluj (kliknij 2x).command` → **Otwórz** → w oknie systemowym potwierdź jeszcze raz **Otwórz**.
3. Gotowe — aplikacja instaluje się do Programów i uruchamia sama.

> Dlaczego prawy przycisk, a nie zwykły dwuklik? macOS ostrzega przy pierwszym uruchomieniu
> czegokolwiek niepodpisanego pobranego z internetu — to jednorazowe, kolejne uruchomienia
> (i aktualizacje) już o to nie pytają.
>
> **Jeśli mimo to zobaczysz „Rzecz «BeKeto Studio» jest uszkodzona"** (starsza instalka albo
> Mac na Apple Silicon bywa surowszy): przeciągnij `BeKeto Studio.app` do Programów, otwórz
> **Terminal** i wklej:
> ```
> xattr -cr "/Applications/BeKeto Studio.app"
> ```
> To usuwa flagę kwarantanny — plik nie jest uszkodzony, to tylko ostrzeżenie systemu dla
> niepodpisanych aplikacji.

## Aktualizacje — automatyczne
Po zainstalowaniu program **sam sprawdza i pobiera nowe wersje** przy uruchomieniu.
Nie musisz nic robić ani instalować ponownie — wystarczy normalnie korzystać z aplikacji.
