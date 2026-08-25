# Co nowego w narzędziach System 10H

> **Dla kogo:** dla Ciebie — osoby, która ma zainstalowany katalog narzędzi System 10H.
> Każda aktualizacja dopisuje tu jeden akapit: **co się zmieniło i co z tego masz**. Bez numerków
> w treści, bez żargonu. Numer wersji jest z boku, żeby dało się dopasować do tego, co masz u siebie.
>
> **Zasada:** jeśli aktualizacja **zabiera** albo **zmienia** coś, czego już używasz, będzie to
> napisane **pierwszym zdaniem** — nie schowane w środku. Czego nie wolno zmieniać po cichu,
> spisaliśmy sobie obok w `KOMPATYBILNOSC.md`.

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

