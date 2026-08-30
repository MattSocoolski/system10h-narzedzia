# Co nowego w narzędziach System 10H

> **Dla kogo:** dla Ciebie — osoby, która ma zainstalowany katalog narzędzi System 10H.
> Każda aktualizacja dopisuje tu jeden akapit: **co się zmieniło i co z tego masz**. Bez numerków
> w treści, bez żargonu. Numer wersji jest z boku, żeby dało się dopasować do tego, co masz u siebie.
>
> **Zasada:** jeśli aktualizacja **zabiera** albo **zmienia** coś, czego już używasz, będzie to
> napisane **pierwszym zdaniem** — nie schowane w środku. Czego nie wolno zmieniać po cichu,
> spisaliśmy sobie obok w `KOMPATYBILNOSC.md`.

---

## 🆕 wersja 0.2.7 (30.08.2026)

**Nic nie znika i nic nie przestaje działać.** Domknięcie tego, co naprawiła 0.2.6 — w dwóch
miejscach, do których wtedy nie zajrzeliśmy.

**`autopilot-instalacja`: opis kroku 2.7 podawał gotową komendę ze ścieżką, która istnieje tylko
przy instalacji z paczki.** Jeśli masz procedurę z katalogu narzędzi, ta jedna komenda
zatrzymałaby Cię kilka kroków po tym miejscu, które naprawiliśmy w 0.2.6. Teraz opis nie podaje
żadnej ścieżki — odsyła do komendy sprawdzającej z samej procedury, a katalog podstawia Claude Code.

**Co z tego masz:** instalacja przechodzi do końca także wtedy, gdy procedurę masz z katalogu.
Jeśli robisz ją z paczki, nic się dla Ciebie nie zmienia.

---

## 🆕 wersja 0.2.6 (30.08.2026)

**Nic nie znika i nic nie przestaje działać.** To wydanie naprawia jedną rzecz, ale taką, która
zatrzymywała od razu na starcie.

**`autopilot-instalacja` działa teraz także wtedy, gdy procedurę masz z katalogu narzędzi, a swój
System w osobnym folderze.** Wcześniej w tym układzie kończyła się natychmiast komunikatem, że nie
znajduje pliku — pliku, który u Ciebie **był**, tylko procedura szukała go w złym miejscu. Szukała
„o tyle a tyle katalogów w górę", a przy instalacji z katalogu narzędzi te dwa foldery nie mają ze
sobą nic wspólnego. Teraz procedura pyta wprost o katalog Twojego Systemu i pracuje na nim.

**Co z tego masz:** jeśli zatrzymała Cię wcześniej ta wiadomość, po aktualizacji przejdzie dalej.
Jeśli nie zatrzymała — nie zauważysz różnicy i nic nie musisz robić inaczej.

**Gdyby znów czegoś nie znalazła**, komunikat mówi teraz po ludzku, czego szuka i gdzie zaglądał,
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

---

<!--
NOTATKA WEWNĘTRZNA (nie dla klienta — usuń przy ewentualnej publikacji jako osobna strona):

Plik założony 24.08.2026 (taśma §B1, ruch (a) itemu DYSTRYBUCJA-SKILLE-PILOT). Powód: klient
dostawał do tej pory wyłącznie numer wersji, a kanał zwrotny jest świadomie wyłączony — więc
aktualizacja bez zdania po ludzku jest dla niego zdarzeniem bez treści. Wzorzec z transkryptu
[44:21]: „Hej, Łukasz właśnie dodał tutaj nową wersję, są dane dla Etiopii i dla Malty (…) czy
chcesz zaktualizować skilla?".

⚠️ TREŚĆ WPISU 0.2.2 JEST DRAFTEM @cto — idzie do klienta, więc przed wysłaniem/publikacją
przechodzi przez @ghost (CLAUDE.md §ZASADY JAKOŚCI OUTPUTÓW: @ghost = gatekeeper komunikacji).
Znacznik [DO PRZEREDAGOWANIA PRZEZ @GHOST] zdejmuje @ghost, nie autor draftu.

⚠️ TO SAMO DOTYCZY WPISU 0.2.6 (30.08.2026): treść jest draftem @cto. Została
opublikowana w katalogu 30.08 na wyraźne polecenie usera („trzeba zaktualizować wtyczkę”),
PRZED przejściem przez @ghost — widoczny znacznik zdjęty przy publikacji, żeby klient nie
czytał naszej kuchni. Jeśli @ghost zmieni brzmienie, poprawka to jeden commit do katalogu:
plik jest dokumentem do wglądu, nie wysyłką, więc korekta nie „dogania” nikogo.

⚠️ TO SAMO DOTYCZY WPISU 0.2.7 (30.08.2026, kilka godzin po 0.2.6): draft @cto, opublikowany
na tę samą zgodę usera — 0.2.7 domyka klasę, którą 0.2.6 zostawiła w połowie, więc jest
dokończeniem tamtej decyzji, nie nową. Widoczny znacznik zdjęty przy publikacji.

Wpisy 0.2.1 i 0.2.0 są CELOWO ubogie: odtworzone z tytułów commitów (b20b2699, 4113f050), bo
notatek wtedy nie prowadziliśmy. Nie dopisuję im treści, której nie zmierzyłem — pusty wpis jest
uczciwszy niż zmyślony (ZASADY ANTYHALUCYNACJI). Od 0.2.2 wpis powstaje RAZEM z wersją.

Kontrakt: kto buduje nową wersję (`zbuduj-plugin-10h.mjs`), ten dopisuje tu akapit W TYM SAMYM
ruchu. Evaluator itemu sprawdza, że numer z manifestu występuje w tym pliku.
-->
