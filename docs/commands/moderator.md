# Moduł moderacji
### skrót modułu: mod

Moduł zawiera szereg poleceń służących do czynności moderatorskich.

Dostępne dla administratorów polecenia:
- move

Gdy użytkownicy spamują wypadało by usunąć ich wiadomości LUB przenieść na odpowiedni kanał.
Przenoszenie wiadomości odbywa się za pomocą poniżej przedstawionej komendy.
Konfiguracja odbywa się poprzez wpisanie polecenia: 
```
[prefix]mod move {messageCount} {channelMention}
```
MessageCount - ilość wiadomości do przeniesienia. Należy ręcznie policzyć ile wiadomości (ostatnich od wiadomości z poleceniem) ma zostać przeniesionych
ChannelMention - kanał na który mają zostać przeniesione wiadomości

Przykład:
[Filmik/Gif]



Objasnienia:

- prefix - zdefiniowany przez Administratora bota - domyślnie jest to !
- channelMention - #nazwa_kanału
- game - obecnie dostępne to td (The Division), custom (Inne gry), td2 (The Division 2)