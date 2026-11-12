# ♠ Licznik pokerowy

Licznik turniejowy (blind timer) do pokera, który **automatycznie podnosi stawki** po upływie czasu poziomu. Działa w przeglądarce na telefonie, tablecie, komputerze i telewizorze. Można go zainstalować jak aplikację i używać bez internetu.

**Otwórz:** https://kamil787pl.github.io/poker/

## Funkcje

- Duży zegar, blindy z żetonami (SB / BB / ante), kolejny poziom i lista kolejnych poziomów z godzinami startu
- Automatyczna zmiana poziomu z gongiem, animacją i komunikatem głosowym po polsku (możesz wybrać głos damski)
- Przerwy, ostrzeżenie minutę przed końcem poziomu i tykanie przez ostatnie 5 sekund
- Panel administracyjny chroniony PIN-em (domyślnie **1234**):
  - sterowanie zegarem: start i pauza, przeskok poziomu, ±1 min, ustawienie czasu, przerwa na żądanie;
  - edytor struktury, 4 gotowe szablony i generator struktury;
  - wpisowe, re-buy, add-on, prowizja i podział nagród;
  - gracze: eliminacje, miejsca, losowanie miejsc przy stole i cofanie ostatniej akcji;
  - kalkulator żetonów: Twój zestaw kolorów i nominałów, rozdanie stacka na gracza, kontrola, na ilu graczy wystarczy;
  - motywy sukna, ustawienia dźwięku i głosu, kopia zapasowa danych.
- Przypomnienie o wymianie żetonów (chip race) na ekranie przerwy i głosem
- Stan zapisuje się automatycznie, więc odświeżenie strony nie przerywa turnieju
- Blokada wygaszania ekranu (Screen Wake Lock)

## Instalacja na telefonie / tablecie

- **Android (Chrome):** otwórz link → menu ⋮ → *Zainstaluj aplikację* / *Dodaj do ekranu głównego*.
- **iPhone / iPad (Safari):** otwórz link → *Udostępnij* → *Do ekranu początkowego*.

Po pierwszym otwarciu aplikacja działa także bez internetu.

## Pliki

| Plik | Opis |
|---|---|
| `index.html` | cała aplikacja (HTML, CSS, JavaScript w jednym pliku) |
| `manifest.webmanifest` | opis aplikacji do instalacji (nazwa, ikony, kolory) |
| `sw.js` | service worker – działanie offline |
| `icons/` | ikony aplikacji |

## Aktualizacja

Po zmianie `index.html` podnieś numer wersji w `sw.js` (np. `const CACHE = 'licznik-v3'`), żeby zainstalowane aplikacje pobrały nową wersję.
