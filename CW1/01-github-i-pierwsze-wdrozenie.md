# Ćwiczenie 1: konto, Codespaces i pierwsze wdrożenie

**Responsive Web Design · UKEN · semestr zimowy 2026/27 · blok 1 (90 minut)**

**Efekt:** masz konto GitHub, własne repozytorium z plikami startowymi, uruchomiony Codespace i stronę opublikowaną pod publicznym adresem.

Podstawy Gita w pigułce: [Ściąga GitHub](sciaga-github.md).

---

## Jak pracujemy

- **Nie instalujemy niczego na komputerze.** Edytor VS Code, terminal i podgląd strony działają w przeglądarce, w usłudze **GitHub Codespaces**. Możesz więc pracować na każdym komputerze, także w domu.
- Przyciski w GitHubie i VS Code mają **angielskie nazwy**. Podajemy je w cudzysłowie, a obok polskie wyjaśnienie.
- Po każdym etapie robisz **commit**, czyli zapisujesz „zdjęcie" projektu z krótkim opisem. Historia commitów to Twój dziennik budowy i podstawa punktów za checkpoint.
- **Ten plik ma format Markdown (`.md`).** Na GitHubie wyświetla się jako ładna strona. Bloki kodu mają w prawym górnym rogu ikonę **kopiowania**: klikasz i wklejasz do edytora, bez ręcznego zaznaczania.

### Słowniczek w pigułce

| Pojęcie | Co znaczy |
|---|---|
| Repozytorium (repo) | Folder projektu z całą historią zmian, przechowywany na GitHubie |
| Commit | Zapisanie zmian z opisem („zdjęcie" projektu w danym momencie) |
| Push / Sync Changes | Wysłanie commitów z Codespaces do repozytorium na GitHubie |
| Codespace | Twoje środowisko pracy w przeglądarce (edytor VS Code + terminal) |
| Deploy / GitHub Pages | Publikacja strony pod publicznym adresem |

---

## Zadanie 1.1: konto GitHub

- [ ] **1. Wejdź na GitHub.** Otwórz [github.com](https://github.com). Jeśli masz już konto, kliknij „Sign in" (zaloguj się) i przejdź do zadania 1.2.
- [ ] **2. Rejestracja.** Kliknij „Sign up" (załóż konto). Podaj swój adres e-mail i kliknij „Continue".
- [ ] **3. Hasło.** Wymyśl hasło (co najmniej 15 znaków albo 8 znaków z cyfrą i małą literą). Zapisz je w bezpiecznym miejscu.
- [ ] **4. Nazwa użytkownika (username).** To adres Twojej strony i wizytówka w portfolio. Najlepiej imię i nazwisko bez polskich znaków, np. `jan-kowalski`. Unikaj pseudonimów typu `xX_killer_Xx`.
- [ ] **5. Weryfikacja.** Rozwiąż krótką zagadkę obrazkową i kliknij „Create account". Na e-mail przyjdzie kod weryfikacyjny, wpisz go na stronie.
- [ ] **6. Plan darmowy.** Jeśli GitHub pyta o plan, wybierz „Continue for free" (darmowy). Pytania o preferencje możesz pominąć: „Skip personalization".
- [ ] **7. Zapisz nazwę.** Zapisz swoją nazwę użytkownika w pliku `notatki.md` (powstanie w zadaniu 1.8) albo na kartce.

> **Uwaga na komputery w sali.** Nie zapisuj hasła w przeglądarce (jeśli zapyta, wybierz „Never" / „Nie"). Na koniec zajęć wyloguj się z GitHuba: ikona profilu w prawym górnym rogu → „Sign out".

---

## Zadanie 1.2: własna kopia projektu (Fork)

Skopiuj repozytorium startowe z konta prowadzącego. Zrobisz z niego własną kopię (**fork**) na swoim koncie na GitHubie.

- [ ] **1. Otwórz repozytorium startowe.** Wejdź w przeglądarce pod adres: `https://github.com/lukaszrosickiuken/RWD_AI26zim` *(uwaga: bez końcówki `.git`)*.
- [ ] **2. Kliknij Fork.** W prawym górnym rogu strony kliknij przycisk **„Fork”** (ikona rozwidlenia).
- [ ] **3. Ustawienia forka.**
  - W polu **„Owner”** upewnij się, że wybrane jest Twoje konto.
  - Pole **„Repository name”** możesz zostawić domyślne lub zmienić na `rwd-2026`.
  - Upewnij się, że zaznaczona jest opcja **„Copy the main branch only”**.
- [ ] **4. Utwórz kopię.** Kliknij zielony przycisk **„Create fork”**.
- [ ] **5. Sukces.** Po chwili GitHub przeniesie Cię do Twojej własnej kopii pod adresem: `github.com/TWOJA-NAZWA/rwd-2026`.

---

## Zadanie 1.3: uruchom Codespace, czyli edytor w przeglądarce

- [ ] **1. Otwórz menu.** Na stronie swojego repozytorium kliknij zielony przycisk „Code".
- [ ] **2. Utwórz Codespace.** Przejdź do zakładki „Codespaces" i kliknij „Create codespace on main" (utwórz codespace na gałęzi main).
- [ ] **3. Poczekaj.** Otworzy się nowa karta z edytorem VS Code. Uruchamianie trwa od 30 sekund do 2 minut. Jeśli pojawi się pytanie o zaufanie do autorów, kliknij „Yes, I trust the authors".
- [ ] **4. Rozejrzyj się.** Po lewej lista plików (Explorer), pośrodku edytor, na dole panel terminala. Kliknij w lewym panelu plik `index.html`, żeby go otworzyć.
- [ ] **5. Okienka.** Powiadomienia i okienka o rozszerzeniach możesz zamknąć krzyżykiem.
- [ ] **6. Podgląd tego pliku.** Otwórz w Codespace plik `cwiczenia/01-github-i-pierwsze-wdrozenie.md` i naciśnij `Ctrl+Shift+V`. Zobaczysz go w formie „ładnej strony", tak jak na GitHubie.

> **Ważne o Codespaces**
>
> - Codespace wyłącza się sam po pewnym czasie bezczynności (domyślnie ok. 30 minut). Nic nie tracisz, zapisane zmiany zostają. Wróć na [github.com/codespaces](https://github.com/codespaces), kliknij nazwę swojego codespace i pracuj dalej.
> - Zmiany w plikach zapisuje się skrótem `Ctrl+S` (włączyliśmy też autozapis). Na GitHuba trafiają dopiero po **commicie i synchronizacji** (zadanie 1.5).
> - Darmowe konto ma miesięczny limit godzin w Codespaces, więc na koniec zajęć **zatrzymaj** codespace: lewy dolny róg, zielony przycisk → „Stop Current Codespace".

---

## Zadanie 1.4: pierwsza zmiana i podgląd strony

- [ ] **1. Edytuj.** W pliku `index.html` zmień tekst `[Twoje imię]` w nagłówku `<h1>` na swoje imię. Dopisz pod nagłówkiem jedno zdanie o sobie w znaczniku `<p>`. Zapisz: `Ctrl+S`.
- [ ] **2. Uruchom podgląd.** Kliknij prawym przyciskiem plik `index.html` na liście plików i wybierz „Open with Live Server". Alternatywa: w prawym dolnym rogu kliknij „Go Live".
- [ ] **3. Zobacz stronę.** Otworzy się nowa karta przeglądarki ze stroną. Jeśli przeglądarka zapyta o otwarcie portu, kliknij „Open in Browser".
- [ ] **4. Sprawdź odświeżanie.** Wróć do edytora, zmień coś w tekście i zapisz (`Ctrl+S`). Strona w podglądzie odświeża się sama.

---

## Zadanie 1.5: pierwszy commit i push

Commit zapisuje zmianę w historii. Sync (push) wysyła ją na GitHuba, żeby była w Twoim repozytorium.

- [ ] **1. Otwórz Source Control.** Kliknij trzecią ikonę na pionowym pasku po lewej (rozgałęzienie, podpis „Source Control", skrót `Ctrl+Shift+G`). Powinna być lista „Changes" z plikiem `index.html`.
- [ ] **2. Wpisz opis commita.** W polu „Message" wpisz opis zmiany, np. `Pierwsza strona z moim imieniem`. Opis ma mówić, **co zrobiłeś(aś)**.
- [ ] **3. Zrób commit.** Kliknij niebieski przycisk „Commit". Jeśli VS Code zapyta „There are no staged changes… commit all?", kliknij „Yes" (albo „Always").
- [ ] **4. Wyślij na GitHub.** Kliknij niebieski przycisk „Sync Changes" (synchronizuj zmiany). Jeśli pyta o potwierdzenie, kliknij „OK".
- [ ] **5. Sprawdź na GitHubie.** Wejdź na `github.com/TWOJA-NAZWA/rwd-2026` w osobnej karcie i odśwież. Nad listą plików będzie Twój opis commita, a po kliknięciu „Commits" zobaczysz historię.

**Wersja z terminala** (działa tak samo). W panelu „Terminal" na dole wpisz po kolei, każdą linijkę zatwierdź klawiszem Enter:

```bash
git add .
git commit -m "Pierwsza strona z moim imieniem"
git push
```

- `git add .` zbiera zmienione pliki,
- `git commit -m "..."` zapisuje je z opisem,
- `git push` wysyła na GitHuba.

---

## Zadanie 1.6: publikacja strony, czyli GitHub Pages

- [ ] **1. Ustawienia.** Wejdź na stronę swojego repozytorium na github.com (nie w Codespaces) i kliknij zakładkę „Settings" (po prawej stronie paska zakładek).
- [ ] **2. Pages.** W menu po lewej kliknij „Pages".
- [ ] **3. Źródło publikacji.** W sekcji „Build and deployment", w polu „Source" wybierz „Deploy from a branch". Niżej w „Branch" wybierz `main` i folder `/ (root)`, potem kliknij „Save".
- [ ] **4. Adres strony.** Odczekaj 1–2 minuty i odśwież stronę ustawień. Pojawi się komunikat „Your site is live at…". Adres ma postać: `https://TWOJA-NAZWA.github.io/rwd-2026/`
- [ ] **5. Sprawdź na telefonie.** Otwórz ten adres na telefonie. Do czego służy w `index.html` linia z `viewport`? Zapisz odpowiedź w `notatki.md`.

---

## Zadanie 1.7: cykl „edycja, commit, publikacja"

- [ ] **1. Powtórz cykl.** Zmień coś w `index.html` w Codespaces, zrób commit i Sync. Odśwież publiczny adres i zanotuj w `notatki.md`, po ilu minutach zmiana się pojawiła.
- [ ] **2. Opisz pojęcia** własnymi słowami w `notatki.md`: *repozytorium*, *commit*, *deploy*.

---

## Zadanie 1.8: notatki w Markdown

Format `.md` (Markdown) to zwykły tekst z prostymi znakami formatowania. Używa go GitHub, dokumentacje programistów i wiele narzędzi, więc warto go znać.

- [ ] **1.** W Codespaces kliknij ikonę „New File" w Explorerze i nazwij plik `notatki.md`.
- [ ] **2.** Wklej poniższy szablon i uzupełnij go:

```markdown
# Moje notatki z RWD

**Nazwa konta GitHub:** twoja-nazwa
**Adres strony:** https://twoja-nazwa.github.io/rwd-2026/

## Ćwiczenie 1

- Po ilu minutach zmiana pojawiła się na stronie: ...
- Dokonane zmiany:
```

- [ ] **3.** Naciśnij `Ctrl+Shift+V`, żeby zobaczyć podgląd. Zrób commit i Sync (opis: `Notatki`). Otwórz plik na GitHubie i zobacz, jak się wyświetla.

Najważniejsze znaki: `#` nagłówek, `##` podnagłówek, `**pogrubienie**`, `*kursywa*`, `-` lista, `` `kod` `` w tekście, ` ``` ` blok kodu, `[tekst](adres)` link. Pełna lista jest w [ściądze](sciaga-github.md#markdown-w-pigułce).

---

## Checkpoint 0: lista kontrolna

- [ ] Mam konto GitHub i własne repozytorium `rwd-2026`.
- [ ] Potrafię uruchomić Codespace i podgląd strony (Live Server).
- [ ] Moja strona działa pod publicznym adresem `github.io`.
- [ ] Mam plik `notatki.md` z odpowiedziami.
- [ ] Wysłałem(am) link do strony w kanale Teams (Ćwiczenia: linki).

## Dla chętnych

- Dodaj w `README.md` 2–3 zdania o projekcie i link do opublikowanej strony (w Markdown: `[opis](adres)`).
- Dodaj do strony zdjęcie z atrybutem `alt` (przeciągnij plik do panelu Explorer).
- Zapytaj AI „Wyjaśnij, co to jest GitHub Pages" i sprawdź odpowiedź w [dokumentacji GitHub](https://docs.github.com/pages).

---

## Na koniec zajęć

- [ ] Wszystkie zmiany są zapisane commitem i zsynchronizowane.
- [ ] Zatrzymałem(am) Codespace („Stop Current Codespace").
- [ ] Wylogowałem(am) się z GitHuba, jeśli pracowałem(am) na komputerze uczelnianym.
