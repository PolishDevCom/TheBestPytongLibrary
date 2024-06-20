# Process Level - poznawanie procesów
Podczas tego procesu skupiliśmy się na:
 - zwalidowaniu scenariuszy i przypadku użycia podczas sortowania
 - odnalezieniu biznesowych subdomen
 - przypisanie ryzyk i wyzwań do procesów
 - odnalezienie granic modularyzacji (żródła prawcy i zbiory regół)

## Dodanie poleceń
![processlevel_add_command_pl.png](../../../assets/processlevel_add_command_pl.png)

Uwagi dodatkowe:
 - zakupiono książkę -> zgłoszono zakupienie książkę
 - Sprawdzono i przyjęto podarowaną książkę -> zgłoszono sprawdzenie i przyjęcie podarowanej książki
 - założono konto klienta biblioteki -> założono konto czytelnika
 - potwierdzono dane użytkownika -> potwierdzono dane czytelnika
 - Wyciągnięto książkę (tymczasowa rezerwacja) -> wyciągnięto książkę do czytelni
 - Odłożono książkę (anulowanie tymczasowej rezerwacji) -> zwrócono książkę z czytelni
 - zmienienino naprawiono książkę -> zgłoszono naprawienie książki
 - zutylizowano książkę -> zgłoszono zutylizowanie książki
 - sprzedano książkę -> zgłoszono sprzedaż książki
 - Zgubiono książkę -> zgłoszono zgubienie książki

## Dodanie reguł
W miejscach gdzie nie wiadomo czy proces ma być kontynułowany dodano reguły które muszą być sprawdzone

Uwaga dodatkowa:
 - zauważono brakujące zdarzenie "dodano raport podarowanej książki"
 - zauważono brakujące zdarzenie "odebrano formularz z prośbą założenie konta czytelnika"
 - zauważono brakujące zdarzenie "zapisano ustawienie systemowe"
 - zauważono brakujące zdarzenie "powiadomioniono użytkownika o anulowaniu rezerwacji"
 - zauważono brakujące zdarzenie "powiadomioniono użytkownika o rozpoczęciu rezerwacji"
 - zauważono brakujące zdarzenie "powiadomienie użytkownika że zarezerwowana książka czeka na odbiór"
 - zauważono brakujące zdarzenie "zapisono osobę która anulowała karę"

Postanowienia:
 - Zastanawialiśmy się czy traktować książki jako pojedyńcze rekordy w tabeli, czy jako pozycje mające ilość sztuk - postanowiliśmy potraktować każdy egzemplaż jako osobny byt, a po fazie MVP jeśli będzie taka potrzeba przeprowadzić normalizację.

![processlevel_rules_part1.png](../../../assets/processlevel_rules_part1.png)
![processlevel_rules_part2.png](../../../assets/processlevel_rules_part2.png)

## Dodaj modele odczytu
