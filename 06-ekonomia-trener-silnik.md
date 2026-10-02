# Ekonomia, trener i silnik meczu

## Ekonomia

Rozliczenie jest tygodniowe (dokładna godzina na Local Schedule twojej ligi).

### Wpływy
- Bilety z meczów u siebie i ze środka tygodnia.
- Sponsorzy: zależą od ligi i liczby kibiców. Nastrój sponsorów widać na stronie ekonomii.
- Sprzedaż zawodników i opłaty nowych kibiców (ok. 30 za osobę) wchodzą jako wpływy tymczasowe.

### Wydatki
- Pensje: 250 bazowo + kwota od skilli i wieku. Obcokrajowiec +20%. Specjalność +10%.
- Utrzymanie stadionu, budowa, sztab, skauci akademii, odsetki od długu.

### Dług
Linia kredytowa ok. 500 000. Po jej przekroczeniu ostrzeżenie o bankructwie i wysokie odsetki. Nie schodź pod zero, jeśli nie musisz.

### Stadion
Cztery typy miejsc. Płacisz utrzymanie co tydzień, nawet przy pustych trybunach.

| Typ | Bilet | Utrzymanie/tydz. | Budowa | Rozbiórka |
|-----|-------|------------------|--------|------------|
| Ławki | 7 | 0,5 | 45 | 6 |
| Zwykłe | 10 | 0,7 | 75 | 6 |
| Zadaszone | 19 | 1 | 90 | 6 |
| VIP | 35 | 2,5 | 300 | 6 |

Każda zmiana pojemności kosztuje dodatkowo 10 000. Istniejące miejsca działają w trakcie budowy.

Podział biletów:
- Liga: wszystko bierze gospodarz.
- Puchar: 67% gospodarz, 33% gość. Ostatnie 6 rund na neutralnym, po połowie.
- Sparingi i baraże: po połowie.

Frekwencja zależy głównie od liczby kibiców. Na starcie nie rozbudowuj stadionu na zapas — puste miejsca tylko zjadają utrzymanie. Rozbudowa ma sens, gdy regularnie wyprzedajesz.

## Trener główny

Nowy klub startuje z trenerem poziomu 3 (zadowalający / passable). Skill trenerski maks. 5 (znakomity / excellent). Leadership osobno, do solidnego (7).

- Skill trenerski: szybkość treningu.
- Leadership: wyższe morale drużyny.
- Styl: ofensywny, defensywny albo neutralny. Wpływa tylko na mecz, nie na trening.

Ofensywny podbija atak i obcina obronę. Defensywny odwrotnie, i obronę podbija trochę mocniej niż ofensywny atak. Neutralny nie rusza żadnej linii. Wiki podaje dla ofensywnego ok. +8% ataku i −11% obrony względem neutralnego. Nowsze opracowania (Ocerin) mówią o +5% ataku i −14% obrony. Asystent taktyczny pozwala zmiękczyć ten rozkład.

Przy treningu bierz wysoki skill i leadership solidny (7), styl neutralny, chyba że świadomie grasz kontrę (defensywny) albo atak (ofensywny).

Ceny zewnętrzne (skill wierszami od słabego do znakomitego, leadership kolumnami od kiepskiego do solidnego), w US$:

| Skill \\ Leadership | 3 | 4 | 5 | 6 | 7 |
|--------------------|---|---|---|---|---|
| 1 | 10k | 10k | 10k | 10k | 10k |
| 2 | 10k | 22,8k | 41,2k | 65,1k | 94,6k |
| 3 | 79,6k | 182,8k | 329,7k | 521k | 757,1k |
| 4 | 268,7k | 617,1k | 1,11 mln | 1,76 mln | 2,56 mln |
| 5 | 4 mln | 4,39 mln | 7,91 mln | 12,5 mln | 18,2 mln |

Stary trener zostaje w kadrze jako zawodnik, nie można go sprzedać ani zrobić znowu trenerem. Albo zostawiasz, albo zwalniasz.

Priorytet kasy: najpierw trener solidny (skill 4, leadership 7, ok. 2,56 mln), potem asystenci 5 i lekarz 5.

## Silnik meczu

Pomoc rozdaje szanse. Posiadanie:

`posiadanie = pomoc_A / (pomoc_A + pomoc_B)`

Same szanse nie idą liniowo. Badania społeczności (HT Press, HTMS) podają coś w rodzaju:

`P(szansa A) = pomoc_A^3 / (pomoc_A^3 + pomoc_B^3)`

Powyżej ok. 65–70% posiadania dokładanie do pomocy daje coraz mniej szans. Wtedy lepiej doić atak albo obronę.

Zwykłych szans w meczu jest rzędu 10, dzielonych między drużyny. Do tego dochodzą stałe fragmenty, kontry, strzały z dystansu i zdarzenia specjalne.

Konwersja szansy na gola to pojedynek sektora ataku z sektorem obrony rywala (atak środek vs obrona środek, lewy atak vs prawa obrona i odwrotnie). Przy równych ocenach prawdopodobieństwo gola jest poniżej 50% (badania HT Press: ok. 42,5% przy formule `0,74 * atak^3 / (0,74 * atak^3 + obrona^3)`). Bezpośredni rzut wolny i strzał z dystansu to pojedynek wykonawcy z bramkarzem, nie ocen sektorów.

Zdarzenia specjalne skalują się z posiadaniem: przy 75% posiadania masz ok. 75% szans na SE, jeśli obie strony mają specjalistów pod ten event.

## Pogoda
Krótko, bo specjałki są w pliku 03:
- Słońce: technical +5%, powerful −5%, quick −5%.
- Deszcz: powerful +5%, technical −5%, quick −5%.
- Nieprzewidywalny odporny na pogodę.

## Narzędzia
- Foxtrick — wtyczka do przeglądarki: oceny, składy, linki do analiz.
- Hattrick Organizer (HO) — składy, przewidywane oceny, analiza rywala, trening.
- HTMS (fantamondi) — statystyki posiadania i konwersji z dziesiątek tysięcy meczów.
- SkillValue — sublevele, filtr transferów, podpowiedź składu.

## Źródła
- hattrick.org podręcznik: Economy, Stadium, Coach
- wiki.hattrick.org: Coach, Scoring opportunities
- HT Press (rozkład szans), HTMS
