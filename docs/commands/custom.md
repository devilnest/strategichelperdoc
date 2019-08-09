# Moduł Wydarzeń dla Dowolnych gier
### skrót modułu: custom

Moduł zawiera szereg poleceń służących do tworzenia wydarzeń dla różnych gier.

Dostępne polecenia dla użytkowników:
- event [alias: e]

W celu umożliwienia użytkownikom tworzenia wydarzeń należy je skonfigurować. Więcej informacji w module konfiguracja: 
Rozpoczęcie tworzenia wydarzenia rozpoczyna się poprzez wpisanie komendy: 
```
[prefix]custom event
```
Po wpisaniu komendy bot przywita się z Tobą wiadomością początkową.
Następnie przeprowadzi przez cały proces tworzenia wydarzenia. Będziesz musiał wykonać parę rzeczy, ponieważ nie wszystko jesteśmy w stanie przewidzieć.

Tak prezentuje się krótka instrukcja korzystania z powyższego polecenia
```
1. Wpisz komendę: [prefiks]]td2 event
2. Podaj nazwę gry
3. Podaj nazwę aktywności w wybranej grze.
4. Podaj maksymalną ilość ludzi mogących dołączyć do wydarzenia.
5. Podaj datę rozpoczęcia wydarzenia:
a. Wpisując : 23:00 utworzysz wydarzenie na obecny dzień na podaną godzinę.
b. Wpisując: 23:00 28-06-2019 uzyskasz czas rozpoczęcia wydarzenia na konkretny dzień.
6. Podaj dodatkowy opis wydarzenia. Jest to krok, który można ominąć wpisując : brak                                     | KROK OPCJONALNY
```
Objasnienia:

- prefix - zdefiniowany przez Administratora bota - domyślnie jest to !
- eventId - identyfikator wydarzenia pozwalający na jego indetyfikację. Identyfikator znajduje się w tytule wydarzenia : Wydarzenie#1