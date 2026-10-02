# Ćwiczenie 2: audyt i responsywna karta wydarzenia

**Responsive Web Design · UKEN · semestr zimowy 2026/27 · blok 2 (90 minut)**

**Efekt:** ocena responsywności cudzych stron i własna responsywna karta wydarzenia, opublikowana w Twoim repozytorium.

Poprzednie ćwiczenie: [Ćwiczenie 1](01-github-i-pierwsze-wdrozenie.md). Podstawy Gita: [Ściąga GitHub](sciaga-github.md).

> **Przed startem:** otwórz swój Codespace (jeśli się wyłączył: [github.com/codespaces](https://github.com/codespaces) → kliknij jego nazwę). Wyniki audytu i Lighthouse zapisuj w pliku `notatki.md` w nowej sekcji `## Ćwiczenie 2`.

---

## Zadanie 2.1: mini-test (5 min)

Odpowiedz krótko na pytania, które pokaże prowadzący. Test służy do dopasowania tempa i **nie jest oceniany**.

---

## Zadanie 2.2: audyt w parach (25 min)

- [ ] **1. Wybór stron.** Wybierz z partnerem dwie strony: jedną instytucji kultury z regionu i jedną wzorcową (np. [gov.uk](https://www.gov.uk)).
- [ ] **2. Narzędzia deweloperskie (DevTools).** W Chrome lub Edge naciśnij `F12`, potem `Ctrl+Shift+M` (tryb urządzenia mobilnego).
- [ ] **3. Trzy szerokości.** Sprawdź 360 px, 768 px i 1280 px. Zapisz notatkę, jeśli masz wątpliwości co do prawidłowego wyswietlania strony. 
- [ ] **4. Lighthouse.** W DevTools wybierz zakładkę „Lighthouse", tryb „Mobile", kliknij „Analyze page load" i zapisz cztery wyniki.
- [ ] **5. Zoom i klawiatura.** Powiększ stronę do 200% (`Ctrl` i `+`), przejdź po niej klawiszem `Tab`.
- [ ] **6. Karta audytu.** Skopiuj tabelę poniżej do `notatki.md` i wypełnij (0 = brak, 1 = częściowo, 2 = dobrze).

```markdown
## Ćwiczenie 2: audyt

| Kryterium | Strona A: ... | Strona B: ... |
|---|---|---|
| 1. Viewport i skalowanie | | |
| 2. Czytelność tekstu bez powiększania | | |
| 3. Brak przewijania poziomego (360 px) | | |
| 4. Duże, wygodne elementy dotykowe | | |
| 5. Najważniejsze informacje w 2 dotknięciach | | |
| 6. Obrazy dopasowane i nie za ciężkie | | |
| 7. Kontrast i hierarchia nagłówków | | |
| 8. Obsługa klawiaturą (Tab), widoczny fokus | | |
| 9. Zoom 200%: nic nie znika | | |
| 10. Lighthouse mobile (wydajność / dostępność / dobre praktyki / SEO) | | |

**Wniosek pary (2 zdania):** ...
```

- [ ] **7. Commit.** Zrób commit z opisem `Audyt stron` i Sync Changes.

---

## Zadanie 2.3: karta wydarzenia

Pliki startowe masz już w swoim repozytorium, w folderze `card`: `index.html` jest gotowy, `style.css` zawiera podpowiedzi, a w `img/` są obrazy. Twoim zadaniem jest napisać wygląd w `style.css`, **etapami**, z commitem po każdym etapie.

Do stylowania card uzyj frameworków **boostrap oraz własnego css** albo **tailwind**

**UWAGA:** Czy aby na pewno style css działa prawidłowo?

- [ ] **0. Uruchom podgląd.** W Explorerze rozwiń folder `karta-wydarzenia`. Kliknij prawym przyciskiem `index.html` w tym folderze → „Open with Live Server". Zobaczysz trzy brzydkie, niestylowane karty. To dobrze, od tego zaczynamy.

---

## Zadanie 2.4: siatka kart

Domyślnie pojedyncza karta rozciąga się na pełną szerokość ekranu, ponieważ nie mamy odpowiedniego **kontenera**. Owiń karty w responsywny kontener `grid`, który zmienia liczbę kolumn w zależności od ekranu:
- **Mobile (domyślnie):** 1 kolumna
- **Tablet (`md:` od 768 px):** 2 kolumny
- **Desktop (`lg:` od 1024 px):** 3 kolumny

1. Dodaj na elemencie nadrzędnym (np. `<section>` lub `<div>` otaczającym karty) klasy:

```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
  <!-- tutaj wklej 3 lub więcej kart -->
</div>
```

---

## Zadanie 2.5 wyślij i zmierz

- [ ] **1. Wyślij zmiany.** Zrób commit i Sync Changes. Odczekaj 1–2 minuty.
- [ ] **2. Otwórz publiczny adres karty:** `https://TWOJA-NAZWA.github.io/rwd-2026/karta-wydarzenia/`
- [ ] **3. Zmierz.** Uruchom Lighthouse (mobile) na tym adresie i wpisz wyniki do `notatki.md`: wydajność / dostępność / dobre praktyki / SEO.

> **Wskazówka:** nie musisz pamiętać składni. Otwórz [MDN Web Docs](https://developer.mozilla.org), wyszukaj „CSS Grid" lub „clamp()" i przeczytaj przykład. Możesz też poprosić AI o wyjaśnienie, a odpowiedź sprawdzić w MDN.

### Dla chętnych

- Tryb ciemny: `@media (prefers-color-scheme: dark)`.
- Układ poziomy karty na szerokim ekranie (container query).
- Czwarta karta i dwa wiersze na tablecie.

---

## Na koniec zajęć

- [ ] Wszystkie zmiany są zapisane commitem i zsynchronizowane (w Source Control nie ma oczekujących zmian).
- [ ] Zatrzymałem(am) Codespace: lewy dolny róg, zielony przycisk → „Stop Current Codespace".
- [ ] Wylogowałem(am) się z GitHuba, jeśli pracowałem(am) na komputerze uczelnianym.

## Checkpoint 1: karta wydarzenia

- [ ] Karta ma czytelną strukturę HTML i działa na szerokościach 360, 768 i 1280 px.
- [ ] Kilka commitów z opisami, widoczna historia etapów.
- [ ] Link do opublikowanej strony i wyniki Lighthouse w kanale Teams.

---
