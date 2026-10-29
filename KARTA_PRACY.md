# Karta pracy — warsztat w parach, ok. 50 minut

Fazy F1–F5 to ścieżka podstawowa. „Bez sufitu" — dla par, którym zostanie czas.
Po **F2, F3 i F5** pilot wpisuje symbol fazy na czacie głównym.

---

## F1 · Wybór wariantu i projekt skilla (8 min, plan mode)

- [ ] Wybierzcie wariant: **A** `/kartkowka` (GIFT + Moodle XML) · **B** `/feedback` (rubryka) ·
      **C** `/plan-zajec` (konspekt). Otwórzcie materiały swojego wariantu z folderu `material/`.
- [ ] Przełączcie agenta w **plan mode** (Shift+Tab) i ZAPROJEKTUJCIE skill rozmową —
      własnymi słowami: co skill ma robić, co dostaje na wejściu, jak DOKŁADNIE ma wyglądać
      wynik (format, struktura, język), czego ma nigdy nie robić.
- [ ] Przeczytajcie plan agenta. Nawigator: czy z tego planu wynika powtarzalny przepis,
      czy jednorazowa przysługa? Poprawcie, zanim zaakceptujecie.

> Wskazówka do wariantu A: skill ma zapisywać kartkówkę w DWÓCH plikach naraz — `.gift`
> (szybki, czytelny) i `.xml` (Moodle XML — niesie parametry, których GIFT nie zapisze:
> punkty, podpowiedzi, losowanie odpowiedzi, komentarz ogólny). Pokażcie agentowi OBA
> wzorce: `przyklady/przyklad.gift` i `przyklady/przyklad.xml` — wzorzec formatu jest
> wart więcej niż opis formatu.

## F2 · Budowa skilla (12 min)

- [ ] Poproście agenta: *„Utwórz ten skill jako plik `.claude/skills/<nazwa>/SKILL.md`
      w tym projekcie, według wzoru z `szablony/SKILL_szablon.md`."*
- [ ] **Przeczytajcie SKILL.md w edytorze** (eksplorator → jeden klik). To są instrukcje,
      które agent będzie czytał przy każdym wywołaniu — czy są jednoznaczne? Czy opis
      (`description`) mówi, KIEDY używać skilla?
- [ ] Poprawcie ręcznie lub poleceniem minimum jedną rzecz (to ćwiczenie z redagowania,
      nie z zaufania).
- [ ] Checkpoint: `F2` na czacie głównym.

## F3 · Test i iteracje (12 min)

- [ ] Nowa sesja agenta (`/clear`) — skill ma działać „na czysto", bez pamięci rozmowy
      o jego budowie. Wywołajcie: `/nazwa` z materiałem wariantu.
- [ ] Oceńcie wynik WOBEC projektu z F1: format się zgadza? struktura? język?
      (Wariant A: powstały OBA pliki — `.gift` i `.xml`? Zgodne ze wzorcami z `przyklady/`?)
- [ ] **Minimum dwie iteracje:** poprawcie SKILL.md (nie prompt!) i wywołajcie ponownie.
      Zmiana ma być w przepisie, nie w jednorazowej prośbie — inaczej to nie skill.
- [ ] ZAMIANA RÓL (jeśli jeszcze nie było komunikatu — zamieńcie się teraz).
- [ ] Checkpoint: `F3` na czacie głównym.

## F4 · Subagent-recenzent (8 min)

Świeże oczy bez świeżego człowieka: poproście agenta o recenzję WYNIKU skilla
przez osobnego podwykonawcę:

> Uruchom subagenta, który oceni plik <wynik> jako [nauczyciel akademicki odbierający
> kartkówkę / student otrzymujący feedback / metodyk oceniający konspekt]. Ma wskazać
> trzy konkrety do poprawy i nie widzieć naszej rozmowy.

- [ ] Przeczytajcie recenzję. Co najmniej JEDNĄ uwagę wprowadźcie do SKILL.md (nie do wyniku!)
      i przetestujcie ponownie.

## F5 · Publikacja (10 min)

- [ ] Commit przez agenta: *„Zapisz projekt w gicie z opisem po polsku: co robi skill
      i jakie decyzje projektowe przyjęliśmy."*
- [ ] Pilot publikuje na SWOIM GitHubie (jak w sesji 2, F5): nowe prywatne repo
      `skill-<nazwa>` przez stronę → agent podpina adres i wypycha.
- [ ] Checkpoint: `F5` + (jeśli chcecie) link na czacie głównym.

---

## Bez sufitu — rozszerzenia

- [ ] **Drugi skill** — wariant, którego nie wybraliście (macie już wprawę: 15 minut?).
- [ ] **Skill parametryczny** — np. `/kartkowka 10 trudna` (liczba pytań, poziom trudności
      jako argumenty).
- [ ] **Twardsze testy** — dajcie skillowi materiał spoza repo (fragment własnego wykładu
      z dysku). Przenośność to test prawdy.
- [ ] **Skill + CLAUDE.md** — dopiszcie do CLAUDE.md regułę współpracującą ze skillem
      (np. "kartkówki zapisuj w wyniki/ z datą w nazwie") i sprawdźcie, czy działają razem.
- [ ] **Recenzent na stałe** — przeróbcie prompt subagenta-recenzenta z F4 na... drugi skill
      `/recenzja`. Tak, skill może uruchamiać subagenta.
- [ ] **Dla ambitnych — MCP w domu:** instrukcja podłączenia pierwszego serwera MCP
      (bezpiecznego, bez danych uczelni) jest w materiałach spotkania; na zajęciach nie
      instalujemy niczego na służbowych maszynach.

---

## Na koniec — do syntezy

Jedno zdanie od pary: **co było trudniejsze — wymyślić przepis czy go zapisać tak,
żeby agent wykonał go bez Was?**
