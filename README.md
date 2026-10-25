# re-openOMSI

Własna edycja openOMSI dla Windows x64, rozwijana niezależnie od repozytorium źródłowego. Zachowane są wymagane informacje o oryginalnym projekcie i licencji.

## Stan: DEV05 (przygotowanie importu źródeł)

Wersja DEV05 z poprawkami znajduje się w paczce źródłowej przygotowanej w ChatGPT. **To repozytorium na razie nie zawiera pełnego drzewa źródeł, więc NIE da się jeszcze zbudować EXE z GitHub Actions.** Import źródeł jest następnym krokiem. Nie uruchamiaj workflow z niekompletnego projektu.

### Funkcje przygotowane w kodzie

- Motyw AMOLED, kolory, tła i pozycjonowanie (źródła, bez testów EXE).
- Profile grafiki dla GTX 1050.
- ANGLE/DirectX 11 bez zmian w działającym backendzie.
- Poprawki GPS i śledzenia gracza w sesji (do testowania po kompilacji).
- Aktualizator wskazujący wyłącznie `kenni-darkus/re-openOMSI`, obsługujący wersje `0.3.41-reopen.N` oraz kanał beta/stable.

### Wydania i automatyczne aktualizacje

Docelowy format pliku wydania: `re-openOMSI-0.3.41-reopen.2-windows-x64.zip`. Wersje beta powinny być oznaczane jako GitHub Pre-release. Oryginalne wydania openOMSI nigdy nie powinny być instalowane jako aktualizacje tej edycji.

**Uwaga:** repo jest prywatne. Aktualizator bez tokenu GitHub nie pobierze prywatnych wydań. Do automatycznych aktualizacji potrzebne są publiczne wydania (np. po upublicznieniu repo albo w oddzielnym publicznym repo dystrybucyjnym). Nie zapisujemy prywatnych tokenów w launcherze.

## Oryginalny projekt

Źródło: https://github.com/openOMSI-org/openOMSI. Kod pochodny musi zachować licencję i wymagane informacje o autorach. Nie jest to oficjalne wydanie openOMSI.
