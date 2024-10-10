# Process Level - poznawanie procesów
Podczas tego procesu skupiliśmy się na:
 - zwalidowaniu scenariuszy i przypadku użycia podczas sortowania karteczek
 - odnalezieniu biznesowych subdomen
 - przypisanie ryzyk i wyzwań do procesów
 - odnalezienie granic modularyzacji (żródła prawdy i zbiory reguł)

## Dodanie poleceń
![processlevel_add_command_pl.png](../../../assets/processlevel_add_command_pl.png)

Uwagi dodatkowe:
 - zakupiono książkę -> zgłoszono zakupienie książkę
 - Sprawdzono i przyjęto podarowaną książkę -> zgłoszono sprawdzenie i przyjęcie podarowanej książki
 - założono konto klienta biblioteki -> założono konto czytelnika
 - potwierdzono dane użytkownika -> potwierdzono dane czytelnika
 - Wyciągnięto książkę (tymczasowa rezerwacja) -> wyciągnięto książkę do czytelni
 - Odłożono książkę (anulowanie tymczasowej rezerwacji) -> zwrócono książkę z czytelni
 - zmieniono naprawiono książkę -> zgłoszono naprawienie książki
 - zutylizowano książkę -> zgłoszono zutylizowanie książki
 - sprzedano książkę -> zgłoszono sprzedaż książki
 - Zgubiono książkę -> zgłoszono zgubienie książki

## Dodanie reguł
W miejscach gdzie nie wiadomo czy proces ma być kontynuowany dodano reguły które muszą być sprawdzone

Uwaga dodatkowa:
 - zauważono brakujące zdarzenie "dodano raport podarowanej książki"
 - zauważono brakujące zdarzenie "odebrano formularz z prośbą założenie konta czytelnika"
 - zauważono brakujące zdarzenie "zapisano ustawienie systemowe"
 - zauważono brakujące zdarzenie "powiadomiono użytkownika o anulowaniu rezerwacji"
 - zauważono brakujące zdarzenie "powiadomiono użytkownika o rozpoczęciu rezerwacji"
 - zauważono brakujące zdarzenie "powiadomienie użytkownika że zarezerwowana książka czeka na odbiór"
 - zauważono brakujące zdarzenie "zapisano osobę która anulowała karę"

Postanowienia:
 - Zastanawialiśmy się czy traktować książki jako pojedyncze rekordy w tabeli, czy jako pozycje mające ilość sztuk - postanowiliśmy potraktować każdy egzemplarz jako osobny byt, a po fazie MVP jeśli będzie taka potrzeba przeprowadzić normalizację.

![processlevel_rules_part1.png](../../../assets/processlevel_rules_part1.png)
![processlevel_rules_part2.png](../../../assets/processlevel_rules_part2.png)

## Dodaj modele odczytu
Zastanowiliśmy się jak powinien wyglądać model odczytu, i w których miejscach go potrzebujemy.

- Model odczytu powinien znajdować się przed komendą.
- Model odczytu to dane które będą zasilać komendę

Dodano modele odczytu:
- odczyt ilości przedłużeń okresu wypożyczenia
- raport z dodanej książki
- whislista
- formularz założenia konta czytelnika - x2
- konto czytelnika - x2
- kary użytkownika - x3
- wypożyczenia użytkownika
- książka
- stan wypożyczenia książki - x5
- termin oddania książki
- lista kar - x2
- lista kar użytkownika - x4

![[Pasted image 20241010224524.png]]
![[Pasted image 20241010224547.png]]
![[Pasted image 20241010224558.png]]
![[Pasted image 20241010224609.png]]
![[Pasted image 20241010224619.png]]
![[Pasted image 20241010224629.png]]

## 