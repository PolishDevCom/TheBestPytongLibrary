# Big Picture - poznawanie z oddali
Podczas tego etapu skupiliśmy się na:
- poznaniu kontekstu systemu bibliotecznego,
- poznaniu ryzyk i wyzwań,
- określeniu złożoności domeny,
- wyznaczeniu procesów biznesowych jako wstępu Process Level.

## Agenda
Do wszystkich etapów potrzebna będzie agenda mówiąca jaka kartka co oznacza, w związku z tym ustaliliśmy agendę.
![agenda.png](../../../assets/agenda.png)

## Cel warsztatu
Podzielił bym tą kategorię na dwie osobne:
 - Rozpoczeliśmy je chcąc nauczyć się odkrywania procesów biznesowych, i zdobycia doświadczenia z Event Stormingiem.
 - Dlatego też postawiliśmy sobie cel zbadania procesów biznesowych biblioteki. I tym na czym się skupiamy to jak najlepsze zaprojektowanie systemu bibliotecznego.

## Zdarzenia
Na tym etapie zrobiliśmy burzę muzgów i dodawaliśmy karteczki opisujące zdarzenia:
 - zakupiono książkę
 - dodano książkę do księgozbioru
 - sprowadzono i przyjęto książkę
 - zniszczono książkę
 - anulowano karę
 - minął termin oddania książki
 - maliczono karę
 - zaplacono karę
 - zgubiono książkę
 - zawieszono kartę biblioteczną
 - zutylizowano książkę
 - sprzedano książkę
 - naprawiono książkę
 - założono konto czytelnika
 - wydano kartę biblioteczną
 - zamknięcie konta czytelnika
 - zarezerwowano książkę
 - wyciągnięto książkę
 - wypożyczono książkę
 - przedłużono okres wypożyczenia
 - zwrócono książkę
 - odłożono książkę

![bigpicture_events_pl.png](../../../assets/bigpicture_events_pl.png)

## Oś czasu
Po uzbieraniu zdarzeń wprowadzono oś czasu, i uporządkowano zdarzenia od najstarszego do najmłodszego.
Gdy zdarzenia które mieliśmy znalazły się na osi czasu, prześledziliśmy je od końca sprawdzając czy zaszły wszystkie inne zdarzenia potrzebne do wystąpienia obecnego.


![bigpicture_timeline_pl.png](../../../assets/bigpicture_timeline_pl.png)

## Źródło zdarzeń
Gdy wiedzieliśmy kiedy zachodzi jakie zdarzenie skupiliśmy się na wskazaniu kto wywołuje dane zdarzenie.

![bigpicture_actors_pl.png](../../../assets/bigpicture_actors_pl.png)

Dodatkowo na tym etapie jeszcze raz patrząc po czasie uznano że warto przedyskutować i zmienić:
- zniszczono wypożyczoną książkę -> zgłoszono zniszczenie wypożyczonej książki
- zniszczono książkę (nie wykryty sprawca) -> zgłoszono zniszczenie książki w księgozbiorze
- dodano zdarzenie "odblokowano konto czytelnika"