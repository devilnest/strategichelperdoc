# Moduł statystyk
### skrót modułu: stats

Moduł zawiera szereg poleceń służących do wyświetlania statystyk z gry The Division 2.

Dostępne dla użytkowników polecenia:
- register
- stats 
- stats pve
- stats pvp

Jak w każdej grze - liczą się statystyki. Nie musisz wejść do gry, aby zobaczyć ile masz kasy, ile wykonałeś strzałów w głowę. Wstarczy, że zarejestrujesz się w bazie bota, a on pobierze statystyki i wyświetli je w przyjaznej formie.
Aby zarejestrować się w bocie należy wykonać polecenie: 
```
[prefix]register [NickNaPlatformieUplay]
```
Bot o ile nie jesteś już zarejestrowany pobierze z API Uplay dane na temat Twojego profilu i wyświetli w postaci wiadomości. 
Bot będzie czekać 5 minut na weryfikację danych i Twoją reakcję pod wiadomością. Po upływie 5 minut i braku reakcji - wiadomości zostają usunięte i rejestrację należy zacząć od początku.

Jeżeli jesteś zarejestrowany już w bocie, ale zmienił Ci się nick i chciałbyś go zaktualizować to polecenie też pozwoli Ci na zmianę nicka. (Nick jest używany w obrębie discorda. Nie pozwala to na zmianę nicka w systemie Uplay)


Po zarejestrowaniu się w bazie bota, będziesz mógł wyświetlić swoje statystyki w grze. Nie są to wszystkie statystyki jakie można wyświetlić jednak jest ich tak dużo, że wyświetlanie ogarniczyło się do kilkunastu. Statstyki możesz podejrzeć za pomocą polecenia
```
[prefix]stats
[prefix]stats pve
[prefix]stats pvp
```
- stats - wyświetla statystyki PvE ORAZ PvP
- stats PvE - wyświetla tylko statystyki PvE (np. ilość kredytów)
- stats PvP - wyświetla tylko statystyki PvP (np. najdłuższy czas statusu Rogue)


Co więcej jeżeli masz znajomego, który jest również zarejestrowany możesz użyć poleceń:

```
[prefix]stats pve @Znajomy
[prefix]stats pvp @Znajomy
```

Po użyciu powyższych poleceń bot wyświetli statystyki gracza pod wartością - @Znajomy.
Oczywiście tylko w przypadku, gdy @Znajomy jest zarejestrowany w bocie.


```
Objasnienia:
- prefix - zdefiniowany przez Administratora bota - domyślnie jest to !
- @Znajomy - @NazwaUżytkownikaZDiscord#1234
- NickNaPlatformieUplay - Twój/Znajomego nick na platformie uplay



Bot przechowuje dane takie jak:
- Twój nick z uplay, ID na uplay, ID na discordzie - wymagane, aby ułatwić używanie pobierania statystyk
- Twoje statystyki - aby nie odpytywać systemu UPLAY co 5 s. Chomiki by nie nadążyły.

Bot również raz dziennie aktualizuje dane z systemu UPLAY dla wszystkich użytkowników w bazie.
```