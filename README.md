# Tracker transportów – Europa

Prosta strona do śledzenia transportów (załadunek/rozładunek, przewoźnik, daty, kontakt, numery rejestracyjne) z mapą tras.

## Jak wgrać na GitHub Pages

1. Utwórz nowe repozytorium na GitHubie (może być prywatne).
2. Wgraj plik `index.html` do głównego katalogu repozytorium.
3. Wejdź w **Settings → Pages**.
4. W sekcji "Build and deployment" wybierz **Deploy from a branch**, branch `main`, folder `/root`.
5. Zapisz — po chwili strona będzie dostępna pod adresem `https://twoja-nazwa.github.io/nazwa-repo/`.

## Ważne ograniczenie

Ta wersja **nie ma wspólnego serwera/bazy danych** — GitHub Pages hostuje tylko statyczne pliki.
Dane są zapisywane lokalnie w przeglądarce (localStorage) każdej osoby osobno — nie są automatycznie
współdzielone między różnymi komputerami/osobami.

Żeby przenosić dane między osobami:
- Użyj przycisku **Eksportuj JSON**, żeby pobrać plik z wszystkimi wpisami.
- Druga osoba może użyć **Importuj JSON**, żeby dodać te wpisy u siebie (duplikaty są pomijane po ID).

## Jeśli chcecie prawdziwej wspólnej bazy danych (widocznej dla wszystkich naraz)

Do tego potrzebny jest backend. Najprostsze, darmowe opcje do dopięcia w przyszłości:
- **Firebase (Firestore)** – darmowy plan, kilka linijek kodu do dodania w `index.html`.
- **Supabase** – darmowy plan, baza Postgres + gotowe API.

Daj znać, jeśli chcesz, żebym dopisał integrację z jedną z tych opcji — wtedy dane będą naprawdę wspólne
dla wszystkich, w czasie rzeczywistym.
