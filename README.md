# Problem pet filozofa (Monitori u C)

Ovaj projekt predstavlja rješenje klasičnog problema **Pet filozofa** pomoću **višedretvene sinkronizacije** u C jeziku koristeći **monitore** (kombinacija `pthread_mutex` i `pthread_cond` varijabli).

## Opis problema

Pet filozofa sjede za okruglim stolom i izmjenjuju se između dvije aktivnosti:
- **Razmišljanje**
- **Jedenje**

Između svakog para filozofa nalazi se **jedna vilica** (ukupno 5 vilica). Da bi filozof mogao jesti, mora uzeti **dvije vilice**: lijevu i desnu.

Cilj je:
- Sinkronizirati pristup vilicama tako da **nema zastoja (deadlock)**.
- Osigurati da **nijedan filozof ne gladuje**.
- Prikazivati **stanja svih filozofa u stvarnom vremenu**.
