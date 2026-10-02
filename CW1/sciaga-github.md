# Git — szybka ściąga: commity i cofanie zmian

---

## 1. Zapisywanie zmian (commit i push)

```bash
git status                           # sprawdź stan plików roboczych
git add .                            # dodaj wszystkie zmiany do indeksu (stage)
git commit -m "Krótki opis zmiany"   # utwórz commit lokalnie
git push                             # wyślij commity do zdalnego repozytorium

git log --oneline                    # skrócona lista commitów: <HASH> <opis>

```markdown
# Git — szybka ściąga: commity i cofanie zmian

---

## 1. Zapisywanie zmian (commit i push)

```bash
git status                           # sprawdź stan plików roboczych
git add .                            # dodaj wszystkie zmiany do indeksu (stage)
git commit -m "Krótki opis zmiany"   # utwórz commit lokalnie
git push                             # wyślij commity do zdalnego repozytorium

```

---

## 2. Podgląd historii

```bash
git log --oneline                    # skrócona lista commitów: <HASH> <opis>

```

---

## 3. Cofanie zmian

| Sytuacja | Polecenie | Działanie |
| --- | --- | --- |
| Porzucenie zmian w jednym pliku (przed commitem) | `git restore <plik>` | Przywraca stan z ostatniego commita (bezpowrotnie). |
| Porzucenie zmian we wszystkich plikach | `git restore .` | Cofa modyfikacje całego drzewa roboczego. |
| Przywrócenie pliku ze starego commita | `git restore --source=<HASH> <plik>` | Wczytuje wersję pliku z commita `<HASH>`; wymaga commita. |
| Bezpieczne odwrócenie commita (nowy commit) | `git revert <HASH>` | Tworzy commit cofający zmiany (dla ostatniego: `HEAD`). |
| Obejrzenie repozytorium w danym punkcie historii | `git switch --detach <HASH>` | Tryb tylko do odczytu (powrót: `git switch main`). |

```

```