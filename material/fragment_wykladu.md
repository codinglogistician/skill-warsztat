# Spektrum autonomii narzędzi AI — fragment wykładu

> Materiał źródłowy do warsztatu. Fragment skryptu z sesji 1 kursu, rozszerzony.

Narzędzia sztucznej inteligencji wspierające pracę z kodem i dokumentami różnią się
przede wszystkim jednym parametrem: **ile decyzji podejmuje narzędzie, a ile człowiek**.
Ten parametr nazywamy autonomią i wygodnie jest myśleć o nim jak o osi.

Na lewym krańcu osi znajduje się **autouzupełnianie** — narzędzie podpowiada kolejny
wyraz lub wiersz, a człowiek zatwierdza każdy znak. Kontrola jest pełna, ale dźwignia
niewielka: tempo pracy rośnie o kilkanaście, może kilkadziesiąt procent.

Dalej na osi leży **czat** — człowiek zadaje pytanie, model odpowiada, generuje fragment
tekstu lub kodu, ale to człowiek kopiuje, wkleja i skleja wynik w całość. Mówimy, że czat
**doradza**. Odpowiedzialność za integrację pozostaje w całości po stronie użytkownika.

Przełom następuje w punkcie, w którym narzędzie zaczyna **wykonywać**: czytać pliki,
planować pracę, wprowadzać zmiany i uruchamiać polecenia. Takie narzędzie nazywamy
**agentem**. Agent interaktywny — na przykład Claude Code — wykonuje pracę etapami,
przedstawia plan, prosi o zgody na operacje i pokazuje różnice w plikach. Człowiek
przestaje być wykonawcą, a staje się **nadzorcą i decydentem**.

Na prawym krańcu osi działają **agenci autonomiczni** — uruchamiani w tle lub w chmurze,
wykonują całe zadanie od początku do końca i zgłaszają się z gotowym wynikiem do przeglądu.
Kontrola człowieka przesuwa się z trybu „na bieżąco" do trybu „przed i po": dokładne
zlecenie na wejściu, krytyczny odbiór na wyjściu.

Kluczowa teza brzmi: **sztuką nie jest praca na maksimum autonomii, lecz dobór punktu
na osi do zadania i stawki**. Zadania o niskiej stawce — prototyp, narzędzie na własny
użytek, szkic — znoszą wysoką autonomię, bo koszt błędu jest mały, a korekta tania.
Zadania o wysokiej stawce — ocenianie studentów, dane osobowe, dokumenty formalne
uczelni — wymagają przesunięcia w lewo: więcej punktów kontroli, obowiązkowy przegląd,
czasem rezygnacja z automatyzacji w ogóle.

Z tej tezy wynikają trzy praktyczne zasady. Po pierwsze, **stawka przed wygodą**: decyzję
o poziomie autonomii podejmujemy od konsekwencji błędu, nie od tego, co szybsze. Po drugie,
**nadzór wymaga czytania**: zgody, plany i różnice w plikach istnieją po to, żeby je czytać —
zatwierdzanie bez lektury to autonomia pełna, tylko udawana. Po trzecie, **delegacja nie
zwalnia z rozumienia**: człowiek, który nie umie ocenić wyniku, nie nadzoruje agenta,
lecz mu wierzy — a wiara nie jest kategorią inżynierską.

Warto też pamiętać, że autonomia narzędzia nie jest cechą stałą. To samo narzędzie może
pracować w różnych punktach osi: agent interaktywny z włączonym trybem planowania działa
„bardziej w lewo", a ten sam agent z automatycznym akceptowaniem zmian — „bardziej w prawo".
Punkt pracy wybiera użytkownik, świadomie albo przez zaniechanie.
