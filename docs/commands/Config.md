
# Moduł konfiguracji
### skrót modułu: config

Moduł zawiera szereg poleceń służących do konfiguracji mechanizmów zawarych w bocie do ich prawidłowego funkcjonowania.

Dostępne dla administratorów polecenia:
- eventChannel
- annoucingChannel
- statsChannel
- bot
- addClan

W celu umożliwienia użytkownikom tworzenia wydarzeń należy je skonfigurować.
Konfiguracja odbywa się poprzez wpisanie polecenia: 
```
[prefix]config eventChannel {channelMention} {game}
```

Opcjonalną funkcjonalnością jest ogłaszanie utworzonych wydarzeń. Opcja przydatna, gdy nasz serwer posiada dedykowany kanał pozwalający na szukanie ludzi do gry.
Po włączeniu tej opcji (ustawieniu kanału) bot wysyła skrót utworzonego wydarzenia na wskazany kanał.
Konfiguracja odbywa się poprzez wpisanie polecenia: 
```
[prefix]config eventChannel {channelMention} {game}
```

W przypadku, gdy na naszym serwerze gracze grają w The Division 2 bot pozwala na wyświetlanie statystyk, aby jednak zapobiec spamowaniu statystykami na każdym kanale należy tą opcję skonfigurować w podobny sposób jak wyżej wymienione opcje.
Konfiguracja odbywa się poprzez wpisanie polecenia: 
```
[prefix]config statsChannel {channelMention}
```

Objasnienia:

- prefix - zdefiniowany przez Administratora bota - domyślnie jest to !
- channelMention - #nazwa_kanału
- game - obecnie dostępne to td (The Division), custom (Inne gry), td2 (The Division 2)