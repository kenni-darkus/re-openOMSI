# re-openOMSI

Nieoficjalna edycja [openOMSI](https://github.com/openOMSI-org/openOMSI) dla Windows x64. Projekt jest oparty na kodzie openOMSI **v0.3.42** (commit `e624dfbfaec0fac92ee78f9eca57bf845544a503`) i udostępniany zgodnie z **AGPL-3.0** (licencja oryginalnych źródeł).

## Pobieranie gry

**[Releases: Windows x64](https://github.com/kenni-darkus/re-openOMSI/releases)**

Wydanie testowe w budowie: **0.3.42-reopen.1 (Beta)**. Link będzie dostępny dopiero po zakończeniu pomyślnej kompilacji i automatycznej publikacji wydania. Niezakończony lub nieudany build nie jest aktualizacją gry.

**[GitHub Actions: postęp kompilacji](https://github.com/kenni-darkus/re-openOMSI/actions/workflows/re-openomsi-build.yml)**

Pierwsze przejście z oryginalnego openOMSI lub wcześniejszego re-openOMSI wymaga **jednorazowego ręcznego pobrania i uruchomienia nowej paczki Windows**. Dopiero skompilowany launcher z tego projektu ma nowy adres aktualizacji; starego launchera nie da się przeprogramować samym dodaniem wydania na GitHubie.

1. Zachowaj kopię działającej instalacji i ustawień.
2. Po pomyślnym buildzie pobierz ZIP z Releases, rozpakuj do osobnego katalogu i uruchom `openomsi.exe`.
3. W launcherze włącz **Aktualizacje → Kanał beta**, żeby otrzymywać testowe wydania tego projektu.
4. Jeśli wszystko działa, można korzystać z tego katalogu zamiast poprzedniej instalacji. Nie usuwaj posiadanych map i pojazdów OMSI 2.

## Co zawiera wersja testowa

- Motyw AMOLED, własne kolory i tła w launcherze.
- Profile graficzne dla laptopa z GTX 1050 (do porównania wydajności).
- Kod zmian GPS i śledzenia graczy (wymaga testów w grze).
- Poprawki licznika przystanku.
- Zachowanie istniejących backendów grafiki; **ANGLE/DirectX 11** dostarczane z oficjalnymi bibliotekami i zweryfikowaną sumą SHA-256.
- Aktualizator kierowany do **kenni-darkus/re-openOMSI**, a nie do wydań oryginalnego openOMSI.

Nie gwarantujemy jeszcze poprawności działania funkcji przed testami na Windows.

## Jak działa build

Repozytorium zawiera niewielki zestaw zmian źródłowych w `overlay/re-openOMSI-DEV07.zip`. Workflow `.github/workflows/re-openomsi-build.yml` pobiera przypięte oryginalne źródła openOMSI v0.3.42, nakłada 29 zmodyfikowanych plików, kompiluje program i przy sukcesie publikuje wydanie beta na GitHub Releases. Nie używa niezweryfikowanych kopii bibliotek DX11.

## Autorstwo i licencja

Kod bazowy należy do autorów [openOMSI](https://github.com/openOMSI-org/openOMSI), udostępniony na AGPL-3.0. Zmiany re-openOMSI to osobna, nieoficjalna odmiana. Przy dystrybucji obowiązują warunki AGPL, w tym dostęp do odpowiednich źródeł i informacji o autorach. Samo osobne repozytorium nie zmienia tych obowiązków.
