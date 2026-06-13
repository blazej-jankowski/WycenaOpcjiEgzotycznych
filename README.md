# Wycena Opcji Egzotycznych — Praca Magisterska

Repozytorium zawiera kompletny skrypt obliczeniowy napisany w języku R na potrzeby pracy dyplomowej magisterskiej pt. **"Wycena Opcji Egzotycznych"** realizowanej na Wydziale Matematyki Politechniki Wrocławskiej.

## Środowisko uruchomieniowe
* **System/Sprzęt:** macOS (Apple MacBook Air M2)
* **Wersja R:** 4.4.2 (2024-10-31)
* **Wymagane pakiety:** `knitr`, `quantmod`, `dplyr`, `xts`, `TTR`, `pracma`

## Zawartość projektu
* `WycenaOpcjiEgzotycznych.R` — główny skrypt zawierający pełną ścieżkę badawczą: od pobrania danych i testów statystycznych, przez kalibrację modeli (CEV, Heston, fBm), aż po silniki wyceny Monte Carlo i drzewa siatkowe.
* `WycenaOpcjiEgzotycznych.Rnw` — plik źródłowy dokumentu (Knitr).
* `bibliografia.bib` — baza literatury w formacie BibTeX.

## Instrukcja uruchomienia
Aby odtworzyć wyniki i wygenerować identyczne tabele oraz wykresy jak w pracy, należy:
1. Upewnić się, że wszystkie wymagane pakiety są zainstalowane (`install.packages(...)`).
2. Uruchomić skrypt główny. Dane dla indeksu S&P 500 zostaną automatycznie pobrane i zamrożone na dzień **2026-06-02**, co gwarantuje pełną powtarzalność wyników numerycznych.
