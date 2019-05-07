# Moduł Wydarzeń dla The Division
### skrót modułu: td

Moduł zawiera szereg poleceń służących do tworzenia wydarzeń dla gry The Division.

Dostępne polecenia dla użytkowników:
- event [alias: e]
- quickjoin [alias: qj]
- join [alias: j]
- remove [alias: r]
- list [W TRAKCIE REALIZACJI]

W celu umożliwienia użytkownikom tworzenia wydarzeń należy je skonfigurować. Więcej informacji w module konfiguracja: 
Rozpoczęcie tworzenia wydarzenia rozpoczyna się poprzez wpisanie komendy: 
```
[prefix]td event
```
Po wpisaniu komendy bot przywita się z Tobą wiadomością początkową.
Następnie przeprowadzi przez cały proces tworzenia wydarzenia. Będziesz musiał wykonać parę rzeczy, ponieważ nie wszystko jesteśmy w stanie przewidzieć.

Tak prezentuje się krótka instrukcja korzystania z powyższego polecenia
```
1. Wpisz komendę: [prefiks]]td event
2. Wybierz typ aktywności, który Cię interesuje klikając w przypisaną wydarzeniu emoji pod wiadomością.
3. Jeżeli dany typ rozgrywki może być rozgrywany w trybie PvP lub PvE, zostaniesz poproszony o wybranie trybu rozgrywki.
4. Wpisz kiedy ma rozpocząć się Twoje wydarzenie.
a. Wpisując : 23:00 utworzysz wydarzenie na obecny dzień na podaną godzinę.
b. Wpisując: 23:00 28-06-2019 uzyskasz czas rozpoczęcia wydarzenia na konkretny dzień.
5. Podaj dodatkowy opis wydarzenia. Jest to krok, który można ominąć wpisując : brak                                     | KROK OPCJONALNY
6. Wpisz nicki graczy, których chcesz dodać do wydarzenia @[nick] , @[nick].  Krok możesz ominać wpisując: brak          | KROK OPCJONALNY
```

W przypadku, gdy użytkownik chce dołączyć do wydarzeniu bezpośrednio po jego ogłoszeniu (wydarzenia mogą być ogłaszane na kanałach np. szukam-graczy), a nie szukać na liście kanałów tekstowych i klikanie w emoji może wpisać polecenie:
```
[prefix]td qj {eventId}
```
Polecenie to dołączy gracza do wydarzenia. W przypadku, gdy *podstawowy* skład jest pełny to gracz zostanie dołączony do składu rezerwowego

Założyciel wydarzenia ma możliwość dołączenia na własną rękę innych graczy do swojego wydarzenia. Jest to również opcja zarezerwowana tylko i wyłącznie dla twórcy wydarzenia. Polecenie można wywołać wpisując:
```
[prefix]td j {eventId} {userMentions}
```
Polecenie to pozwala na dołączenie graczy do wydarzenia. W pierwszej kolejności uzupełniany jest skład *podstawowy*, a następnie skład rezerwowy.
Objasnienia:

- prefix - zdefiniowany przez Administratora bota - domyślnie jest to !
- eventId - identyfikator wydarzenia pozwalający na jego indetyfikację. Identyfikator znajduje się w tytule wydarzenia : Wydarzenie#1
- userMentions - lista użytkowników, których bot ma dołączyć do wydarzenia wprowadzne w postaci: @Bot, @Bot