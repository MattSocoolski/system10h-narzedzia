# Co nowego w narzędziach System 10H

> **Dla kogo:** dla Ciebie — osoby, która ma zainstalowany katalog narzędzi System 10H.
> Każda aktualizacja dopisuje tu jeden akapit: **co się zmieniło i co z tego masz**. Bez numerków
> w treści, bez żargonu. Numer wersji jest z boku, żeby dało się dopasować do tego, co masz u siebie.
>
> **Zasada:** jeśli aktualizacja **zabiera** albo **zmienia** coś, czego już używasz, będzie to
> napisane **pierwszym zdaniem** — nie schowane w środku. Czego nie wolno zmieniać po cichu,
> spisaliśmy sobie obok w `KOMPATYBILNOSC.md`.

---

## 🆕 wersja 0.3.0 (31.08.2026)

**Nic nie znika i nic nie przestaje działać.** Dochodzi jedna nowa procedura — i mówię o niej
od razu wprost, bo jako jedyna w tym katalogu pracuje w interesie nas obu, nie tylko Twoim.

**Skaner Okazji** przegląda Twoje środowisko i składa krótki raport: gdzie Twoja sieć i Twój
biznes spotykają się z tym, co robię ja — tak, żeby zarobiły obie strony. Wynik to gotowy tekst
maila do mnie. **Nic sam nie wysyła i nic u Ciebie nie zapisuje**: ma dostęp wyłącznie do czytania
plików, więc nie jest w stanie zrobić nic więcej, nawet gdyby ktoś go o to poprosił. Wysyłasz Ty
albo nie wysyłasz wcale. Jeśli nie zobaczy nic sensownego, powie to wprost — pusty wynik jest tu
poprawną odpowiedzią, nie porażką.

Procedura **nie zgłasza się sama**; odpala się, kiedy o nią poprosisz. Jedyny wyjątek: gdy właśnie
zobaczyłeś podsumowanie tego, co Twój system dla Ciebie zrobił, asystent może **raz** wspomnieć,
że taka rzecz istnieje. Powiesz „nie" — temat jest zamknięty i nie wraca.

**Co z tego masz:** jeśli kogoś ze swojej sieci widzisz w tym, czym się zajmuję, masz gotowy
sposób, żeby to opisać w pięć minut zamiast układać maila od zera. Zasady rozliczenia ustalamy
indywidualnie, w rozmowie — procedura żadnych kwot ani procentów nie podaje i nie wylicza.

---

## 🆕 wersja 0.2.8 (31.08.2026)

**Nic nie znika i nic nie przestaje działać.** Ta aktualizacja naprawia błąd, który na świeżo
podłączonej skrzynce zatrzymywał Autopilota przy każdym nowym mailu.

**Wpis skrzynki tworzony przy instalacji nie zawierał ustawienia, którego Autopilot bezwzględnie
wymagał** — i zamiast powiedzieć o tym po ludzku, Autopilot wywracał się z technicznym komunikatem
(„Cannot read properties of undefined"). Teraz skrzynka bez tego ustawienia dostaje bezpieczną
domyślną pracę: Autopilot **tylko sygnalizuje** nowe wiadomości (odpowiedzi na Twoje maile
i nadawców z Twoich kart kontaktów), a **żadnych szkiców nie tworzy sam**, dopóki świadomie tego
nie włączysz. Opis pól wpisu skrzynki mówi też teraz wprost, co wpisać w miejscu katalogu kart
kontaktów, gdy kart jeszcze nie masz.

**Co z tego masz:** świeża instalacja na nowej skrzynce działa od pierwszego maila — ostrożnie,
bez samodzielnego pisania, dopóki sam nie zdecydujesz inaczej.

---

## 🆕 wersja 0.2.7 (30.08.2026)

**Nic nie znika i nic nie przestaje działać.** To domknięcie poprzedniej aktualizacji: w tym samym
miejscu została jeszcze jedna rzecz, do której wtedy nie zajrzeliśmy.

**`autopilot-instalacja`: w opisie jednego z pierwszych kroków była wpisana gotowa komenda ze
ścieżką, która istnieje tylko przy instalacji z paczki.** Jeśli procedurę masz z katalogu narzędzi,
ta jedna komenda zatrzymałaby Cię parę kroków dalej niż to, co poprawiliśmy poprzednio. Teraz opis
nie podaje żadnej ścieżki: odsyła do komendy sprawdzającej z samej procedury, a właściwe miejsce
podstawia już Claude Code.

**Co z tego masz:** instalacja przechodzi do końca także wtedy, gdy procedurę masz z katalogu. Jeśli
robisz ją z paczki, u Ciebie nic się nie zmienia.

---

## 🆕 wersja 0.2.6 (30.08.2026)

**Nic nie znika i nic nie przestaje działać.** Ta aktualizacja naprawia jedną rzecz, ale taką, która
zatrzymywała od razu na starcie.

**`autopilot-instalacja` działa teraz także wtedy, gdy procedurę masz z katalogu narzędzi, a swój
System w osobnym folderze.** Wcześniej w tym układzie kończyła się od razu komunikatem, że nie
znajduje pliku. Plik u Ciebie **był**, tylko procedura szukała go w złym miejscu: liczyła katalogi
w górę od siebie, a przy instalacji z katalogu narzędzi te dwa foldery nie mają ze sobą nic
wspólnego. Teraz procedura pyta wprost o folder Twojego Systemu i pracuje na nim.

**Co z tego masz:** jeśli zatrzymał Cię wcześniej ten komunikat, po aktualizacji pójdzie dalej.
Jeśli nie zatrzymał, nie zauważysz różnicy i nic nie musisz robić inaczej.

**Gdyby procedura znów czegoś nie znalazła**, powie teraz po ludzku, czego szuka i gdzie zaglądała,
zamiast wypisywać surowe ścieżki.

---

## 🆕 wersja 0.2.5 (26.08.2026)

**Nic nie znika i nic nie przestaje działać.** Dochodzi jedna procedura, i to taka, którą do dziś
mieliśmy tylko u siebie.

**`autopilot-instalacja`** — przeprowadza przez uruchomienie Autopilota na skrzynce od początku do
końca: trzynaście kroków z zatrzymaniem w miejscu, gdzie hasło wpisuje **wyłącznie właściciel
skrzynki**, i z odmową pójścia dalej, jeśli sprawdzenie serwera wypadnie źle. Zapamiętuje, gdzie
skończyliście — więc przerwana instalacja wznawia się w tym samym miejscu, także po zamknięciu
komputera.

Czym się różni od `autopilot`: tamta odpowiada na pytanie **„czemu nie ma szkiców"** przy
skrzynce już podłączonej, ta prowadzi przez **pierwsze uruchomienie**. Jeśli robisz to sam,
zacznij od `autopilot-instalacja`, a `autopilot` zostaw sobie na później.

Do tej pory ta procedura jechała wyłącznie w paczce instalacyjnej i nie było jej w katalogu —
świadomie, bo dopóki nikt nie przeszedł jej z żywym człowiekiem, wystawianie jej byłoby
rozdawaniem instrukcji, której nikt nie sprawdził w praktyce. Pierwsze przejście z klientem
odbyło się **19 sierpnia** i zatrzymało się na danych serwera pocztowego po stronie dostawcy, a
nie na samej procedurze. Dlatego wchodzi teraz.

---

## 🆕 wersja 0.2.4 (26.08.2026)

**Nic nie znika i nic nie przestaje działać.** Dochodzą dwie nowe procedury — wpisujesz ich nazwę,
gdy ich potrzebujesz, i same się nie odzywają.

**`autopilot`** — prowadzi Cię przez podłączenie poczty do Autopilota i przez diagnozę „czemu nie
ma szkiców". Pilnuje trzech rzeczy, na których to zwykle pęka: żeby hasło nigdy nie przeszło przez
asystenta, żeby czytanie poczty nie oznaczało jej jako przeczytanej, i żeby powtórzenie kroku nie
dopisało tej samej skrzynki dwa razy. **Dwie skrzynki w jednym programie pocztowym** (na przykład
iCloud i Gmail obok siebie) to dla Systemu dwie osobne skrzynki — procedura przeprowadzi Cię przez
obie. Sam program pocztowy nie ma tu nic do rzeczy: System łączy się z serwerem obok niego, więc
szkic pojawia się u Ciebie sam.

**`pamiec-po-znaczeniu`** — o wyszukiwaniu w Twoich plikach po znaczeniu, na modelu działającym na
Twoim komputerze. Zaczyna się od pytania, **czy w ogóle tego potrzebujesz**: asystent czyta Twoje
pliki tak czy owak, a indeks zaczyna coś dawać dopiero przy dużej ilości materiału. Jeśli
procedura skończy się na „na razie niepotrzebne", to jest jej prawidłowy wynik, nie porażka.

Jedno zdanie, żeby nie powstało nieporozumienie z poprzedniej wersji: model wyszukiwania liczy
**u Ciebie** i indeksowana treść nie wychodzi na zewnątrz. **To dotyczy wyszukiwania, nie całego
Systemu** — Autopilot, pisząc szkic odpowiedzi, korzysta z modelu w chmurze na Twoim koncie.

Przy okazji dopisaliśmy w instrukcji rzecz, której wcześniej tam nie było: **komendy Systemu
wymagają Node.js** (zalecana wersja 22 LTS, `https://nodejs.org`). Bez niego żadna z nich nie
ruszy, a komunikat „command not found" znaczy właśnie to — nie awarię Systemu.

---

## 🔄 wersja 0.2.3 (25.08.2026)

**Instrukcja narzędzia do audytu obiecywała więcej, niż to narzędzie robi.** W czterech miejscach było
w niej napisane, że nic nie wychodzi poza Twój komputer. Tak nie jest, dlatego to zdanie stąd znika.

Jak jest naprawdę: **Pliki wyniku zostają u Ciebie i wysyłasz je Ty — treść skanu trafia do dostawcy
modelu na Twoim koncie, tak samo jak przy każdej innej pracy z asystentem.**

Co to oznacza w praktyce? Cztery pliki, które powstają z audytu (`tech_stack.json`,
`tech_stack_human.md`, `profile.md`, `workflow.md`), zostają na Twoim dysku. Narzędzie samo z siebie
nie wysyła ich nigdzie i nikomu, więc to Ty decydujesz, czy w ogóle komuś je pokażesz. Ale treść,
którą asystent czyta w trakcie skanowania, idzie do dostawcy modelu na Twoim koncie. Dokładnie tak
samo jak wtedy, gdy zwyczajnie z nim pracujesz: pytasz o coś, wklejasz dokument, prosisz o poprawkę.

Piszę o tym wprost, bo tamto zdanie mogło wpłynąć na Twoją decyzję, co w ogóle zeskanować. To nie
jest poprawka stylistyczna.

W samym narzędziu nie zmienia się nic. Nic nie przestaje działać, nic nie musisz robić, zmienił się
wyłącznie opis.

---

## 🔄 wersja 0.2.2 (17.08.2026)

**Nic nie przestaje działać. Nie musisz nic robić.**

Audyt, który robisz narzędziem, zapisuje teraz w wyniku **prawdziwą wersję narzędzia**. Wcześniej
wpisywał tam wersję sprzed dwóch poprawek, a wynik wyglądał dokładnie tak samo, więc nie było jak
tego wychwycić.

To jedyne miejsce, po którym da się później stwierdzić, którą wersją powstał Twój audyt. Więc kiedy
odsyłasz wynik do analizy, wiadomo, na czym stał.

Krótko: to samo narzędzie, ten sam sposób użycia, pewniejszy ślad w wyniku.

---

## wersja 0.2.1 (16.08.2026)

Wydanie porządkowe przed udostępnieniem katalogu. Zmiany po naszej stronie, bez wpływu na sposób
korzystania.

## wersja 0.2.0 (09.08.2026)

Pierwsza wersja katalogu instalowanego jednym kliknięciem — zamiast plików wysyłanych mailem.
