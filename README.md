# RS: Red Shift

**RS: Red Shift** to mała, samodzielna gra walki w przeglądarce. Wybierz pojedynek z botem albo lokalną walkę dla dwóch osób. Wyprowadź cios, utrzymaj gardę i wykorzystaj uraken w odpowiednim momencie.

Gra jest inspirowana tematyką boksu i sztuk walki przedstawioną przez [Backfist](https://backfist.pl/). Nie jest oficjalnym produktem ani grą tego klubu.

## Funkcje

- Tryb **Solo**: gracz walczy z botem sterowanym przez komputer.
- Tryb **Lokalnie**: dwie osoby grają na jednym komputerze, korzystając ze wspólnej klawiatury lub przycisków dotykowych na wąskim ekranie.
- Cios prosty, cross, blok, unik oraz specjalny cios **uraken (backfist)**.
- Paski zdrowia i skupienia, 99-sekundowa runda, nokaut lub zwycięstwo po upływie czasu oraz możliwość rewanżu.
- Responsywny interfejs i arena rysowana na elemencie Canvas.

## Uruchomienie

Projekt nie wymaga instalowania zależności, serwera ani procesu budowania. Otwórz plik [`index.html`](index.html) bezpośrednio w przeglądarce.

Gra korzysta z HTML, CSS, JavaScript i Canvas 2D. Nie używa zewnętrznych bibliotek ani plików graficznych.

## Sterowanie

| Akcja | Gracz 1 | Gracz 2 |
| --- | --- | --- |
| Ruch w lewo / prawo | `A` / `D` | `←` / `→` |
| Unik | `W` | `↑` |
| Blok | `S` | `↓` |
| Cios prosty | `F` | `J` |
| Cross | `G` | `K` |
| Uraken | `H` | `L` |

Naciśnij `Spację`, aby rozpocząć walkę lub uruchomić rewanż. Na wąskich ekranach dostępne są przyciski ekranowe; panel Gracza 2 pojawia się w trybie lokalnym.

## Zasady walki

Każdy zawodnik zaczyna ze 100 punktami zdrowia. Zwycięstwo następuje przez nokaut albo po upływie 99 sekund. Wtedy wygrywa zawodnik z większą liczbą punktów zdrowia; jeśli wynik jest równy, walka kończy się remisem.

| Technika | Obrażenia | Dodatkowe informacje |
| --- | ---: | --- |
| Cios prosty | 8 | Szybki cios o krótkim zasięgu. |
| Cross | 13 | Mocniejszy cios z dłuższym przygotowaniem. |
| Uraken / backfist | 22 | Dłuższy zasięg i przygotowanie; kosztuje 35 punktów skupienia. |

Skupienie zaczyna się na poziomie 42 punktów. Trafienia i zablokowane ciosy pomagają je odzyskać. Blok ogranicza otrzymywane obrażenia, a unik na krótko sprawia, że cios przeciwnika może chybić.

## Jak działa tryb Solo

Bot zbliża się lub odsuwa zależnie od dystansu i wybiera ciosy, blok albo unik. Ataki rozstrzygają się po krótkim czasie przygotowania: znaczenie mają zasięg, pozycja, blok i unik przeciwnika.

## Pliki projektu

- [`index.html`](index.html) — cała gra: struktura strony, style, grafika Canvas i logika rozgrywki.
- `README.md` — instrukcja projektu.

## Co nowego

- Dodano grę z trybem Solo przeciw botowi i lokalnym trybem dla dwóch graczy, wraz z ciosami, blokiem, unikiem i urakenem.
- Ujednolicono nazwę gry, areny i postaci pod marką **RS: Red Shift**; zawodnicy noszą nazwy Red i Shift.
