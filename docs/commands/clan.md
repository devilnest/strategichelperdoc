# Moduł Klanów
### skrót modułu: clan

Moduł zawiera szereg poleceń służących do tworzenia klanów na discordzie.

Dostępne polecenia dla użytkowników:
- register
- register channel
- change leader
- show members
- update clans
- add new member
- remove member

W celu umożliwienia użytkownikom tworzenia wydarzeń należy je skonfigurować. Więcej informacji w module konfiguracja: 
Rozpoczęcie tworzenia wydarzenia rozpoczyna się poprzez wpisanie komendy: 
```
[prefix]clan register {clanMention} {leaderMention}
```
Komenda pozwala na rejestrację w bocie klanu z określonym liderem {leaderMention}
```
[prefix]clan changeLeader {clanMention} {leaderMention}
```
Komenda pozwala na aktualizację roli i użytkownika w klanie {clanMention} czego skutkiem jest zmiana dowódctwa klanu i ustawienia jako nowego leadera użytkownika {leaderMention}

```
[prefix]clan showMembers
```
Komenda jako wynik zwraca w wiadomości prywatnej dla lidera klanu listę użytkowników jego klanu.
Lista użytkowników jest budowana na podstawie aktualnie przypisanych ról dla użytkowników Discorda.
Rola według której są szukani użytkownicy to rola przypisana do lidera klanu. Nazwa roli jest zapisana na podstawie wcześniej uruchomionej komendy : clan register

```
[prefix]clan updateClans
```
Komenda pozwala na aktualizację danych w bocie.
Sam Discord nie pozwala tworzyć klanów, więc w przypadku ręcznych akcji przypisania ról (np. przed Administrację) może zajść niespójność pomiędzy tym co "wie" bot, a jaki jest stan faktyczny na serwerze. W celu wyrównania poziomu informacji należy uruchomić komendę.
W planach jest automatyczna aktualizacja w godzinach nocnych.

```
[prefix]clan addMember {userMention}
```
Komenda pozwala na dodanie użytkownika do klanu.
Komenda może być wyłącznie uruchomiona przez Lidera klanu.
Jako wynik komenda wysyła dwie wiadomości:
1. Na kanał na którym została wyzwolona jest wysyłana wiadomość o pozytywnym rozpatrzeniu kandydatury
2. W wiadomości prywatne do kandydata do klanu zawierającą informację do którego klanu został przyjęty oraz na jakim serwerze Discorda

W przypadku, gdy ktoś próbuje dodać użytkownika do swojego klanu, ale użytkownik ten należy już do innego klanu na serwerze - również otrzyma stosowny komunikat.

W planach: Umożliwienie Administracji wykonywanie tej komendy

```
[prefix]clan removeMember {userMention}
```
Komenda pozwala na usujnięcie użytkownika do klanu.
Komenda może być wyłącznie uruchomiona przez Lidera klanu.
Bot w przypadku jak w komendzie: addMember również wysyła dwie wiadomości


```
[prefix]clan registerChannel
```
Komenda pozwala na przypisanie kanału do klanu i umożliwienie tworzenia na nim Wydarzeń. Takie wydarzenia nie ogłaszają się na kanałach (szukam-ludzi-do-gry)
Komenda może być wyłącznie uruchomiona przez Lidera klanu.