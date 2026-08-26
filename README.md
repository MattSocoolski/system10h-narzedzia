# System 10H — narzędzia dla klientów

Katalog narzędzi [System 10H](https://system10h.com) dla klientów z wdrożonym Cyfrowym Bliźniakiem.

## Instalacja (2 komendy w Claude Code)

W Claude Code wpisz kolejno:

```
/plugin marketplace add MattSocoolski/system10h-narzedzia
/plugin install system10h@system10h
```

Wymagany Claude Code w wersji **2.1.224 lub nowszej** (sprawdzisz komendą `claude --version` w terminalu).

Instalacja jest weryfikowana kryptograficznie: jeśli pobrana paczka różni się od opublikowanej choćby o bajt, Claude Code odmówi instalacji.

## Aktualizacje

Nowe wersje ogłaszamy mailem. Po otrzymaniu wiadomości wpisz:

```
/plugin marketplace update system10h
/plugin update system10h@system10h
```

## Co jest w środku

- **`audit-skill`** — audyt integracji technologicznej Twojego środowiska Bliźniaka. Skill jest bezpłatny; produktem System 10H jest analiza wyników, raport i rozmowa o wnioskach — [szczegóły oferty](https://system10h.com).
- **`autopilot-instalacja`** — przeprowadza przez pierwsze uruchomienie Email Autopilota na Twojej skrzynce: krok po kroku, z zatrzymaniem tam, gdzie hasło wpisujesz wyłącznie Ty, i z zapamiętaniem miejsca, w którym skończyliście.
- **`autopilot`** — dla skrzynki już podłączonej: dokłada kolejną (na przykład Gmail obok iCloud) i odpowiada na pytanie „czemu nie ma szkiców".
- **`pamiec-po-znaczeniu`** — o wyszukiwaniu w Twoich plikach po znaczeniu, na modelu liczącym na Twoim komputerze. Zaczyna od pytania, czy w ogóle tego potrzebujesz.

> Dwie procedury Autopilota opisują **podłączenie** poczty i działają u Ciebie. Sam Autopilot, pisząc szkic odpowiedzi, korzysta z modelu w chmurze na Twoim koncie — tak samo jak wtedy, gdy sam wklejasz asystentowi tekst do poprawienia.

## Zasady

- Pliki w tym katalogu są przeznaczone dla klientów System 10H — patrz [LICENSE](LICENSE).
- Ten kanał działa w jedną stronę: nic z Twojego komputera nie jest nigdzie wysyłane.
- Pytania: [system10h.com](https://system10h.com)
