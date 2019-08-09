
# Moduł "zdrowia"
### skrót modułu: health

Moduł zawiera szereg poleceń służących do sprawdzenia stanu działania bota.

Dostępne dla administratorów polecenia:
- check
- eventsStatus

Jako, że bot posiada różne funkcjonalności które działają w tle to w przypadku, gdy użytkownik chciał wiedzieć co się dzieje z botem należy użyć polecenia:
Konfiguracja odbywa się poprzez wpisanie polecenia: 
```
[prefix]health check
```
W zwrotce użytkownik otrzymuje informację o aktualnie działających wątkach: Stan operacji (działa/nie działa) oraz ostatnia wiadomość przesłana przez funkcję


Przydatnym poleceniem do weryfikacji wydarzeń na serwerze oraz dlaczego użytkownik1 klikając dołącz nie zostaje dołączony do wydarzenia należy użyć komendy:
```
[prefix]health eventsStatus
```
W zwrotce użytkownik otrzyma informację o wydarzeniach przechowywanych w bazie (tylko aktywnych i tylko numery) jak i tych, które bot obsługuje (np. po restarcie maszyny, restarcie zawieszonej usługi)



Objasnienia:

- prefix - zdefiniowany przez Administratora bota - domyślnie jest to !
- channelMention - #nazwa_kanału
- game - obecnie dostępne to td (The Division), custom (Inne gry), td2 (The Division 2)