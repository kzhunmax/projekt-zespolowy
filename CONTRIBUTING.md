# Zasady pracy zespołu

Zasady dotyczą wszystkich członków zespołu i obowiązują od 28.10.2026. 

Opis projektu, skład zespołu, role i strukturę repozytorium znajdziesz w [README.md](README.md).

## 1. Przebieg pracy nad zadaniem

1. Weź zadanie w Jirze i zmień status na **W TOKU**.
2. Utwórz gałąź z aktualnego `main`.
3. Pracuj, commituj często i w małych porcjach.
4. Otwórz Pull Request do `main` i wypełnij szablon.
5. Zmień status zadania na **RECENZJA**.
6. Po akceptacji zrób **squash merge**, a zadanie przenieś na **ZROBIONE**.

Do `main` nie wolno wypychać zmian bezpośrednio. Wyjątków nie ma.

## 2. Nazwy gałęzi

Format: `KAN-<numer>-krotki-opis` (małe litery, bez polskich znaków, myślniki).

Przykład: `KAN-12-diagram-przypadkow-uzycia`.

## 3. Commity

Format: `KAN-<numer>: krótki opis w trybie rozkazującym`

Przykłady:
- `KAN-12: dodaj scenariusze PU dla klienta`
- `KAN-20: popraw nazwy statusów zgodnie ze słownikiem`

Zasady: jedna logiczna zmiana na commit, opis do 72 znaków, język polski.

## 4. Pull Request i przegląd

- Jeden PR dotyczy jednego zadania Jira.
- Recenzent: PR-y Maksyma sprawdza Alla lub Yulian, PR-y pozostałych sprawdza Maksym.
- Do scalenia wymagana jest **1 akceptacja**.
- Recenzja powinna zająć ok. 5 minut i opiera się na checkliście z szablonu PR.
- Jeśli nie ma recenzji w ciągu 24 godzin, autor przypomina na Telegramie.
- Uwagi recenzenta autor poprawia w tej samej gałęzi. Scala autor po akceptacji.

## 5. Konwencje dokumentacji

- Na początku każdego pliku: `Autor: Imię Nazwisko`.
- Identyfikatory: `WF-01`, `WNF-01` (wymagania), `PU-01` (przypadki użycia), `TC-01` (przypadki testowe). Nie zmieniamy numerów po zatwierdzeniu.
- Nazwy ról i statusów zlecenia są **takie jak w słowniku** (Nowe, Przypisane, W realizacji, Zakończone, Zamknięte).
- Każdy diagram: plik `.drawio` **oraz** `.png` w `docs/assets/`, osadzony w odpowiednim pliku `.md`.
- Makiety są w Figmie; w repozytorium zostaje link i eksport PNG.
- Dokument końcowy powstaje z Markdown → DOCX → PDF. **Nie edytujemy ręcznie wygenerowanego DOCX poza stroną tytułową i układem**; zmiany treści wprowadzamy w Markdown.

## 6. Definition of Done

Zadanie jest ukończone, gdy:
- [ ] artefakt jest w `main` przez zaakceptowany PR,
- [ ] ma autora i jest zgodny ze słownikiem,
- [ ] źródła diagramów (`.drawio`) i eksporty (`.png`) są w repozytorium,
- [ ] odnosi się do właściwych WF/WNF/PU (tam, gdzie dotyczy),
- [ ] zadanie w Jirze ma status **ZROBIONE**.
