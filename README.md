# Advanced-software-engineering

POLITECHNIKA LUBELSKA
WYDZIAŁ ELEKTROTECHNIKI
I INFORMATYKI
KIERUNEK STUDIÓW
INFORMATYKA
Przedmiot: Zaawansowana Inżynierii Oprogramowania
Raport z wykonania projektu pt.
Express Paczka
Autorzy:
Karol Hetman
Michał Goluch
Michał Grzeszuk
Grupa: IO 5.2
Opiekun: dr inż. Marek Miłosz, profesor uczelni
Lublin, 2021/2022
1
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Podział czynności 3
Krótka charakterystyka systemu 4
Specyfikacja aktorów 5
Historyjki użytkownika 6
Wymagania funkcjonalne 8
Wymagania niefunkcjonalne 10
Obiekty istotne z punktu widzenia systemu 11
Przypadki użycia 19
Scenariusze przypadków użycia 21
Diagram przypadków użycia 30
Diagram klas 31
Diagramy sekwencji 32
Przygotowanie paczki do nadania - Karol Hetman 32
Odebranie paczki - Karol Hetman 33
Dostarczenie paczek - Michał Grzeszuk 34
Rozpoczęcie pracy kuriera - Michał Grzeszuk 35
Zgłoszenie usterki towaru - Michał Goluch 36
Śledzenie paczki - Michał Goluch 37
Diagramy aktywności 38
Przygotowanie paczki do nadania - Karol Hetman 38
Odebranie paczki - Karol Hetman 39
Dostarczenie paczek - Michał Grzeszuk 40
Rozpoczęcie pracy kuriera - Michał Grzeszuk 41
Zgłoszenie usterki towaru - Michał Goluch 42
Śledzenie paczki - Michał Goluch 43
Diagram rozlokowania 44
Zintegrowany Program Rozwoju Politechniki Lubelskiej
PODZIAŁ CZYNNOŚCI
● Michał Grzeszuk - Kierownik zespołu, Dyrektor ds. Dystrybucji i Logistyki
● Karol Hetman - Analityk Systemu Komputerowego
● Michał Goluch - Dyrektor Zakładu Produkcyjnego
Zintegrowany Program Rozwoju Politechniki Lubelskiej
KRÓTKA CHARAKTERYSTYKA SYSTEMU
Express Paczka to aplikacja, która pozwala każdemu zostać dostawcą paczek. Nasza aplikacja
oferuję przewóz paczek na terenie całej Polski. Zatrudniamy i szkolimy kierowców. Aby
rozpocząć pracę w naszej firmie należy założyć konto w aplikacji, okazać potrzebne
dokumenty, przejść krótkie szkolenie i już można ruszać w trasę.
Wyróżniamy się szybkością dostarczania paczek. Nasi kurierzy jeżdżą 24 godziny na dobę.
Również bardzo przykładamy uwagę do jakości naszego transportu. Każda paczka
przewożona jest w bezpieczny sposób oraz dbamy o to aby nie została uszkodzona w
transporcie lub w trakcie kontaktu z paczkomatem.
Dział administracji odpowiada za poprawnie działanie aplikacji. Odpowiada za
bezpieczeństwo i poprawność danych w systemie. Zajmuję się również sprawdzaniem kont
kierowców - ich postępów, ilości ukończonych przejazdów oraz uszkodzeń jakie
spowodowali.
Dział Produkcji dba o rozładunek paczek na magazynie. Następnie są one
segregowane oraz rozdzielane na konkretne działy, z których wyruszają hurtowo do
konkretnych miast.
Dział logistyki zajmuje się porządkiem wśród floty naszych kierowców. Każdy
kierowca, aby rozpocząć pracę musi przejść testy oraz okazać potrzebne dokumenty.
Każdemu kierowcy w aplikacji przysługuje auto służbowe lub jest w stanie jeździć swoim
autem, które spełnia określone wymogi.
Kierowcy, którzy wożą paczki miedzy magazynami zatrudniani są na pełen etat.
Paczki przewożone są w przypadku kiedy są przydzielone one do dostarczenia do innej
placówki. Kierowcy jeżdżą naszymi specjalnie oznaczonymi samochodami ciężarowymi.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
SPECYFIKACJA AKTORÓW
● Administrator - osoba odpowiedzialna za utrzymanie, konfigurowanie i
zarządzanie systemem. Posiada konto o wysokich uprawnieniach dające mu
możliwość administrowania funkcjami i procesami występującymi w systemie.
● Kierowca - osoba odpowiedzialna za transport paczek pomiędzy sortowniami
rozmieszczonymi na terenie kraju. Jest pracownikiem etatowym i do
wykonywania swojej pracy wykorzystuje firmowy samochód.
● Kurier - osoba rozpoczynająca pracę przy użyciu aplikacji. Odpowiada za stan
techniczny auta oraz bezpieczeństwo paczek. Przewozi paczki między
paczkomatami lub przewozi je do magazynu. Może sam zdecydować jaki
paczkomat chce obsłużyć.
● Pracownik magazynu - osoba odpowiedzialna za przenoszenie paczek
pomiędzy samochodami transportowymi na terenie magazynu.
● Klient - osoba korzystająca z systemu w celu nadania lub odebrania paczki. Do
interakcji z systemem wykorzystuje aplikację mobilną.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
HISTORYJKI UŻYTKOWNIKA
1. Jako “Administrator” chciałbym mieć możliwość zalogowania się do systemu aby
mieć możliwość wykonywania swojej pracy.
2. Jako “Administrator” chciałbym mieć możliwość zarządzania kontami innych
użytkowników systemu informatycznego.
3. Jako “Administrator” chciałbym mieć możliwość dostępu oraz edycji bazy danych
żeby móc wprowadzać do systemu nowe dane oraz modyfikować dane już istniejące.
4. Jako “Kierowca” chciałbym otrzymać informację o tym którym samochodem mam
jechać aby dostarczyć paczki.
5. Jako “Kierowca” chciałbym otrzymać informację o lokalizacji magazynu do którego
mam dostarczyć paczki.
6. Jako “Kierowca” chciałbym mieć możliwość zgłoszenia zrealizowania dostawy aby
pracownicy sortowni mogli rozładować mój samochód.
7. Jako “Kierowca” chciałbym mieć możliwość podania powodu opóźnienia lub
uszkodzenia towaru jeżeli takie wystąpi.
8. Jako “Pracownik magazynu” chciałbym, by informacje o przesyłce wyświetlały się w
systemie po zeskanowaniu kodu QR.
9. Jako “Pracownik magazynu” chciałbym, żeby system informatyczny wyświetlał
informacje o tym, gdzie ma zostać skierowana paczka w zależności od jej statusu,
abym wiedział dokąd ją przetransportować.
10. Jako “Pracownik magazynu” chciałbym mieć możliwość potwierdzenia odbioru i
przekazania dalej przesyłki, aby zaktualizować informacje o lokalizacji przesyłki w
systemie.
11. Jako “Klient” chciałbym mieć możliwość śledzenia statusu przesyłki.
12. Jako “Klient” chciałbym mieć możliwość przekierowania paczki.
13. Jako “Klient” chciałbym, żeby aplikacja pokazywała położenie paczkomatów na
mapie.
14. Jako “Klient” chciałbym mieć możliwość nadania paczki w paczkomacie z pomocą
aplikacji.
15. Jako “Klient” chciałbym, żeby system informatyczny generował etykiety które mają
być umieszczone na paczce.
16. Jako “Klient” chciałbym mieć możliwość odebrania paczki z paczkomatu z pomocą
aplikacji.
17. Jako “Kurier” jestem zobowiązany poinformować swojego przełożonego o możliwych
zdarzeniach losowych, które wydłużają czas dostawy paczki.
18. Jako “Kurier” chciałbym, aby system informatyczny umożliwiał mi wybranie zlecenia
odebrania/dostarczenia paczki z listy dostępnych zleceń.
19. Jako “Kurier” chciałbym, aby system informatyczny wskazywał mi miejsca
dostarczenia paczek.
20. Jako “Kurier” chciałbym, aby system informatyczny pozwalał mi w łatwy sposób
otworzyć skrytkę w paczkomacie w celu odebrania lub włożenia paczki do
paczkomatu.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
21. Jako “Kurier” chciałbym, aby system informatyczny automatycznie zmieniał status
paczki po jej włożeniu lub wyjęciu z paczkomatu.
22. Jako “Kurier” chciałbym, za pomocą systemu informatycznego sprawdzać o jakim
priorytecie jest dana paczka.
23. Jako “Kurier” chciałbym mieć możliwość zgłoszenia problemów z funkcjonowaniem
paczkomatu.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
WYMAGANIA FUNKCJONALNE
W ramach projektowanego systemu, dla aktora „Kurier” przewidziano następującą
funkcjonalność:
1. Logowanie do aplikacji - rozpoczęcie pracy i przydzielenie auta do kierowcy.
2. Wyszukiwanie punktów odbioru - szukanie przez kierowców zleceń do odbioru.
3. Odbieranie paczek - przesłanie przez system informatyczny do kierowcy informacji o
tym, który paczkomat zawiera paczki do odebrania.
4. Dostarczanie paczek - przesłanie przez system informatyczny do kierowcy informacji
o tym gdzie ma dostarczyć daną paczkę.
5. Zgłoszenie uszkodzenia towaru - przesłanie przez system informatyczny do
administratora informacji odnośnie uszkodzenia paczki.
6. Zgłaszanie awarii paczkomatu - przesłanie do systemu informatycznego informacji o
uszkodzeniu lub awarii paczkomatu.
W ramach projektowanego systemu, dla aktora „Pracownik magazynu” przewidziano
następującą funkcjonalność:
1. Wyświetlanie danych o przesyłce - po zeskanowaniu kodu QR paczki wyświetlają się
informacje o paczce, między innymi o tym, gdzie trzeba przetransportować paczkę na
terenie magazynu.
2. Potwierdzenie odbioru przesyłki - po zeskanowaniu kodu QR paczki w systemie
powinna zostać zaktualizowana informacja o lokalizacji paczki tym samym
potwierdzając jej dotarcie do określonej sortowni.
3. Potwierdzenie nadania przesyłki - przesłanie do systemu informatycznego informacji
o miejscu do którego została nadana paczka.
W ramach projektowanego systemu, dla aktora “Klient” przewidziano następującą
funkcjonalność:
1. Nadanie paczki - wykorzystanie systemu informatycznego do nadania paczki w
wybranym przez klienta paczkomacie.
2. Wybór priorytetu - wybór priorytetu z jakim ma być nadana paczka.
3. Śledzenie paczki - funkcjonalność umożliwiająca śledzenie aktualnego statusu i
lokalizacji przesyłki.
4. Przekierowanie - zmiana paczkomatu, do którego ma zostać doręczona paczka.
5. Odebranie paczki - wykorzystanie systemu informatycznego do odebrania paczki w
wybranym przez klienta paczkomacie.
6. Ustawienie metody płatności - powiązanie karty bankowej z kontem klienta.
7. Wykonanie płatności - opłacenie przesyłki przez klienta.
W ramach projektowanego systemu, dla aktora „Kierowca” przewidziano następującą
funkcjonalność:
1. Przyjęcie zlecenia - Przesłanie do systemu potwierdzenia o odebraniu zlecenia na
Zintegrowany Program Rozwoju Politechniki Lubelskiej
przewóz przesyłek
2. Raport z przewozu - Złożenie raportu na temat dostarczonych paczek do magazynu
docelowego.
3. Dokumentacja - Przesyłanie przez system informatyczny faktur paliwowych.
4. Zgłoszenie uszkodzenia towaru - przesłanie przez system informatyczny informacji
odnośnie uszkodzenia paczki.
W ramach projektowanego systemu, dla aktora “Administrator” przewidziano następującą
funkcjonalność:
1. Logowanie - funkcjonalność związana z uzyskaniem dostępu do treści i
funkcjonalności przeznaczonych dla administratora systemu.
2. Dodawanie pracowników do systemu - możliwość dodawania pracowników do
systemu oraz nadawania im odpowiednich ról, np. administrator, pracownik sortowni
itd. Role określają uprawnienia użytkownika systemu i związane z tym dostępne
funkcjonalności systemu dla tego użytkownika.
3. Zarządzanie pracownikami - W ramach tej funkcjonalności przewidziano możliwość
zarządzania kontami pracowników. Administrator ma możliwość dezaktywacji konta
pracownika przy jednoczesnym zachowaniu wszystkich danych na jego temat,
zresetowanie hasła i loginu na prośbę pracownika oraz edytowania jego danych.
Ponadto administrator może edytować uprawnienia pracowników.
4. Zarządzanie przesyłkami - administrator ma możliwość ręcznego wprowadzania i
edytowania statusu przesyłki, oraz do momentu ustawienia statusu paczki na “w
realizacji” Opcja zmiany punktu doręczenia przesyłki jest realizowana na zlecenie
klienta w przypadku gdy ten zmienił zdanie lub pomylił się przy wybieraniu
pierwotnego punktu doręczenia przesyłki.
5. Zarządzanie paczkomatami i flotą samochodów - funkcjonalność związania z
dodawaniem i usuwaniem z systemu paczkomatów i samochodów oraz możliwość
zmiany ich statusu.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
WYMAGANIA NIEFUNKCJONALNE
1. Jako serwer webowy system powinien wykorzystywać Apache HTTP Server.
2. System powinien wykorzystywać MySQL w roli systemu zarządzania bazami danych.
3. Jako język programowania po stronie serwera powinien być wykorzystany język PHP.
4. W przypadku aplikacji mobilnej na system android wykorzystywanym językiem
programowania powinna być Java.
5. W przypadku aplikacji mobilnej na system iOS wykorzystywanym językiem
programowania powinien być Swift.
6. System powinien zapewniać stopień ciągłej dostępności na poziomie 99.9% czasu
działania.
7. System powinien odpowiadać na żądanie użytkownika w czasie nie dłuższym niż 1,5
sekundy.
8. Użytkownik w aplikacji powinien bez problemu znaleźć interesującą go przesyłkę a
następnie sprawdzić jej status bez wchodzenia w interakcję z działem obsługi.
9. Aplikacja mobilna powinna działać na urządzeniach z androidem w wersji Lollipop
(5.0) i nowszych.
10. Aplikacja mobilna powinna działać na urządzeniach z systemem iOS w wersji 13 i
nowszych.
11. Aplikacja mobilna powinna być zintegrowana z systemem płatności Google Pay.
12. Aplikacja mobilna powinna posiadać jednorodną oprawę graficzną.
13. Aplikacja mobilna powinna posiadać udogodnienia dla osób niepełnosprawnych.
14. Hasło użytkownika nie może być wyświetlane w formie zwykłego tekstu.
15. Hasło użytkownika powinno być przechowywane w bazie danych w formie skrótu.
16. W roli funkcji haszującej powinna być wykorzystana funkcja bcrypt.
17. Dostęp do serwerów i baz danych powinni mieć tylko użytkownicy z odpowiednimi
uprawnieniami.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
OBIEKTY ISTOTNE Z PUNKTU WIDZENIA SYSTEMU
Placówka
Nazwa atrybutu Opis atrybutu
Nazwa Nazwa placówki
Adres Adres placówki na który składa się miasto, ulica, kod pocztowy i numer
budynku.
Dane
kontaktowe
Dane kontaktowe do tej placówki na które składają się numer telefonu
oraz adres mailowy.
Typ Określa czy dana placówka to sortownia czy biuro.
Paczkomat
Nazwa atrybutu Opis atrybutu
Adres Adres paczkomatu na który składa się ulica, kod pocztowy oraz numer
o ile paczkomat go posiada.
Placówka Placówki pod którą podlega dany paczkomat.
Liczba skrytek Określa liczbę wszystkich skrytek danego paczkomatu.
Liczba zajętych
skrytek
Określa liczbę zajętych skrytek danego paczkomatu.
Status Status paczkomatu, określa czy paczkomat funkcjonuje.
Szerokość
geograficzna
Szerokość geograficzna na jakiej znajduje się dany paczkomat.
Długość
geograficzna
Długość geograficzna na jakiej znajduje się dany paczkomat.
Skrytka
Nazwa atrybutu Opis atrybutu
Oznaczenie Oznaczenie danej skrytki w paczkomacie.
Status Określa czy skrytka jest wolna, zajęta, zarezerwowana, otwarta lub
wyłączona.
Gabaryt Określa maksymalny gabaryt paczki jaki może się zmieścić w danej
Zintegrowany Program Rozwoju Politechniki Lubelskiej
skrytce.
Gabaryt paczki
Nazwa atrybutu Opis atrybutu
Oznaczenie Oznaczenie danego gabarytu paczki.
Wysokość Maksymalna wysokość danego gabarytu paczki.
Szerokość Maksymalna szerokość danego gabarytu paczki.
Długość Maksymalna długość danego gabarytu paczki.
Paczka
Nazwa atrybutu Opis atrybutu
Data utworzenia Data dodania paczki do systemu, jeszcze przed nadaniem paczki w
paczkomacie.
Data nadania Data nadania paczki w paczkomacie.
Data odebrania Data odebrania paczki z paczkomatu przez odbiorcę.
Data odebrania
przez kuriera
Data odebrania paczki z paczkomatu nadania przez kuriera w celu
przekazania jej do sortowni.
Data doręczenia
przez kuriera
Data doręczenia paczki do paczkomatu odbioru przez kuriera.
Nadawca Osoba która nadała paczkę.
Odbiorca Osoba do której została nadana paczka.
Paczkomat
nadania
Paczkomat wybrany przez nadawcę w procesie generowania etykiety
z którego zostanie nadana paczka.
Paczkomat
odbioru
Paczkomat wskazany przez odbiorcę do którego ma być dostarczona
paczka.
Skrytka nadania Skrytka do której nadawca włożył paczkę w danym paczkomacie.
Skrytka odbioru Skrytka w danym paczkomacie do której kurier włożył paczkę.
Priorytet Priorytet paczki wybrany przez odbiorcę w trakcie opłacania przesyłki.
Gabaryt paczki Gabaryt danej paczki. Pozwala na określenie jak dużej skrytki wymaga
dana paczka do nadania.
Status Status paczki. Paczka może mieć następujące statusy: W
Zintegrowany Program Rozwoju Politechniki Lubelskiej
przygotowaniu, nadana, oczekuje na odebranie, odebrana od
nadawcy, wysłana z oddziału, przyjęta w oddziale, w doręczeniu,
gotowa do odbioru, odebrana, zwrócona, anulowana.
Kod QR Kod QR nadawany przesyłce za pomocą którego można odebrać ją z
paczkomatu.
Opis Miejsce na dodatkowe informacje/uwagi dotyczące przesyłki.
Uszkodzenie Opcjonalna informacja o uszkodzeniu paczki jeżeli takie nastąpiło.
Próby odbioru Zlicza ile razy podjęto próbę odbioru paczki.
Samochód
Nazwa atrybutu Opis atrybutu
Marka Marka samochodu.
Model Model samochodu.
Typ Typ samochodu określający czy jest to samochód ciężarowy czy bus
dostawczy lub inny dostępny typ.
Numer
rejestracyjny
Numer rejestracyjny pojazdu.
Numer VIN Numer VIN pojazdu.
OC_od Data przedłużenia ubezpieczenia OC.
OC_do Data wygaśnięcia obecnego ubezpieczenia.
Przegląd_od Data wykonania przeglądu.
Przegląd_do Data ważności przeglądu.
Rok produkcji Rok produkcji danego samochodu.
Ładowność Określa maksymalną ładowność samochodu wyrażoną w kilogramach.
Status Określa status samochodu. Samochód może być dostępny, w
załadunku, w trasie lub niedostępny.
Placówka
macierzysta
Identyfikator placówki która odpowiada za dany samochód.
Placówka
aktualnego
pobytu
Identyfikator placówki w której obecnie jest zaparkowany dany
samochód firmowy.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Pracownik Etatowy
Nazwa atrybutu Opis atrybutu
Imię Imię pracownika.
Nazwisko Nazwisko pracownika.
Płeć Płeć danego pracownika.
Data urodzenia Data urodzenia danego pracownika.
Pesel Pesel danego pracownika.
Data
zatrudnienia
Data zatrudnienia danego pracownika.
Adres Adres zamieszkania danego pracownika.
Email Adres e-mail danego pracownika.
Telefon Telefon kontaktowy do danego pracownika.
Placówka Placówka w której jest zatrudniony dany pracownik.
Dane
uwierzytelniające
Dane uwierzytelniające pozwalające pracownikowi na zalogowanie się
do systemu.
Dezaktywowane Określa czy konto pracownika zostało dezaktywowane.
Rola Określa jakie uprawnienia w danym momencie posiada konto
pracownika.
Szczegóły zatrudnienia
Nazwa atrybutu Opis atrybutu
Stanowisko Stanowisko na którym pracuje dany pracownik.
Stanowisko od Data rozpoczęcia pracy na danym stanowisku.
Stanowisko do Data zakończenia pracy na danym stanowisku. Określa datę kiedy
pracownik zmienił stanowisko pracy lub w przypadku rozwiązania
umowy lub jej zakończenia jest to data odejścia pracownika z pracy.
Wypłata Wypłata jaką otrzymuje comiesięczne pracownik, dotyczy tylko
pracowników etatowych, kurierzy są rozliczani na innych zasadach.
Zatrudniony od Data zatrudnienia pracownika.
Zatrudniony do Data faktyczna odejścia pracownika z pracy lub data zakończenia
obowiązywania umowy o pracę.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Kurier
Nazwa atrybutu Opis atrybutu
Imię Imię danego kuriera.
Nazwisko Nazwisko danego kuriera.
Płeć Płeć danego kuriera.
Data urodzenia Data urodzenia danego kuriera.
Pesel Pesel danego kuriera.
Data
zatrudnienia
Data zatrudnienia danego kuriera.
Data odejścia Data odejścia z pracy danego kuriera.
Adres Adres zamieszkania danego kuriera.
Email Adres e-mail danego kuriera.
Telefon Numer telefonu danego kuriera.
Placówka Placówka dla której pracuje dany kurier.
Dane
uwierzytelniające
Dane uwierzytelniające pozwalające kurierowi na zalogowanie się do
systemu.
Aktywny Określa czy dany kurier w tym momencie pracuje.
Aktywność
Nazwa atrybutu Opis atrybutu
Aktywny od Czas rozpoczęcia pracy przez kuriera w danym dniu.
Aktywny do Czas zakończenia pracy przez kuriera w danym dniu.
Czy swój
samochód
Określa czy kurier podczas danej aktywności korzysta ze swojego
samochodu czy z samochodu firmowego.
Kurier Kurier którego dotyczy dana aktywność
Samochód Samochód z którego korzysta kurier podczas danej aktywności.
Wypłata kuriera
Nazwa atrybutu Opis atrybutu
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Kwota Kwota jaką dostaje kurier za pracę jest wyliczana na podstawie zleceń
jakie wykonał podczas danej aktywności.
Aktywność
kuriera
Aktywności za jakie kurier otrzymuje wypłatę.
Zlecenie
Nazwa atrybutu Opis atrybutu
Czas
rozpoczęcia
Data rozpoczęcia danego zlecenia. Zlecenie polega na odebraniu
paczki przez kuriera z jednego punktu np. paczkomatu i dostarczenia
ich do drugiego punktu np. sortowni.
Czas
zakończenia
Data zakończenia danego zlecenia.
Paczka Identyfikator paczki której dotyczy dane zlecenie.
Opis Miejsce na dodatkowe uwagi dotyczące zlecenia.
Miejsce
odebrania
Miejsce z którego paczka została odebrana, tym miejscem może być
paczkomat lub sortownia.
Miejsce
dostarczenia
Miejsce do którego paczka została dostarczona.
Transport
Nazwa atrybutu Opis atrybutu
Data
rozpoczęcia
Data rozpoczęcia transportu, tj. data wyjechania samochodu z
sortowni.
Data
zakończenia
Data zakończenia transportu, tj. data dojechania samochodu do
sortowni.
Sortownia
nadania
Sortownia z której wyruszyła dana paczka.
Sortownia
docelowa
Sortownia do której transportowana jest paczka.
Kierowca Pracownik odpowiedzialny za transport przesyłki.
Samochód Samochód wykorzystywany do przetransportowania przesyłki.
Paczka Paczka która jest transportowana.
Opis Miejsce na dodatkowe uwagi związane z danym transportem
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Klient
Nazwa atrybutu Opis atrybutu
Imię Imię danego klienta
Nazwisko Nazwisko danego klienta.
Płeć Płeć danego klienta.
Data urodzenia Data urodzenia danego klienta.
Mail Adres e-mail klienta na który może być wysłany kod odbioru paczki.
Numer telefonu Numer telefonu klienta na który może być wysłany kod odbioru paczki.
Adres Adres zamieszkania danego klienta.
Dane
uwierzytelniające
Dane uwierzytelniające umożliwiające klientowi zalogowanie się do
systemu.
Data utworzenia
konta
Data utworzenia konta przez klienta.
Data ostatniego
logowania
Data ostatniego logowania się klienta do swojego konta.
Karta bankowa Karta bankowa powiązana z kontem klienta.
Płatność
Nazwa atrybutu Opis atrybutu
Kwota Kwota jaką klient zapłacił za nadanie paczki.
Data płatności Data wykonania płatności.
Klient Klient który dokonał płatności
Paczka Paczka za której nadanie klient zapłacił.
Faktura
Nazwa atrybutu Opis atrybutu
Numer faktury Unikalny numer faktury.
Data
wystawienia
Data wystawienia danej faktury.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Kwota Kwota całościowa na jaką wystawiona była faktura.
Asortyment
faktury
Określa za co została wystawiona faktura.
Asortyment faktury
Nazwa atrybutu Opis atrybutu
Nazwa Nazwa pojedynczej pozycji na fakturze.
Ilość Określa ile sztuk danej pozycji zostało kupionych.
Cena Cena za jedną sztukę danej pozycji na fakturze.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
PRZYPADKI UŻYCIA
Lista przypadków użycia dla “Administratora”:
1. Utworzenie konta dla nowego pracownika - dodanie do systemu wewnętrznego
nowego pracownika.
2. Dezaktywacja konta pracownika - usunięcie konta danego pracownika.
3. Dodanie danych nowego obiektu - dodanie rekordu do bazy danych.
4. Edycja danych istniejącego obiektu - usuwanie i zmienianie danych istniejących
rekordów w bazie danych.
5. Weryfikacja konta kuriera - zweryfikowanie nowo założonego konta przez osobę
która chce zostać kurierem w Express Paczka.
Lista przypadków użycia dla “Kurier”:
1. Utworzenie konta Kuriera - rejestracja poprzez aplikację zgłaszająca chęć danej osoby
do podjęcia pracy jako kuriera w Express Paczka.
2. Rozpoczęcie pracy kuriera - rozpoczęcie pracy przez kuriera polegające na
zalogowaniu się do aplikacji i uzupełnieniu wszystkich danych dotyczących dnia
pracy.
3. Wyświetlenie listy zleceń - wyświetlanie przez aplikację mobilną listy wszystkich
dostępnych zleceń na obszarze pracy kuriera.
4. Przyjęcie zlecenia - wybranie z listy zlecenia na odbiór bądź dostarczenie przesyłek i
rozpoczęcie jego realizacji.
5. Dostarczenie paczek - dostarczenie przez kuriera paczek do paczkomatu.
6. Zgłoszenie utrudnień w zleceniu - zgłoszenie nieprzewidzianego przypadku w
aplikacji mobilnej.
7. Potwierdzenie dostarczenia paczek - potwierdzenie dostarczenia paczki w aplikacji
mobilnej
8. Utworzenie konta kuriera - tworzenie konta za pomocą aplikacji mobilnej
Lista przypadków użycia dla “Pracownik Magazynu”:
1. Przekazanie paczki kierowcy - zeskanowanie kodu QR paczki na stanowisku
przeładunkowym
2. Wydanie paczki kurierowi - zeskanowanie kodu QR paczki na stanowisku paczek
wydanych do dostarczania
3. Zgłoszenie usterki towaru - zeskanowanie kodu QR paczki oraz zaznaczenie
problemów z odbiorem na ekranie komputera
4. Transport paczki na terenie magazynu - zeskanowanie kodu QR paczki oraz
zaznaczenie pomyślnego odbioru.
Lista przypadków użycia dla “Kierowca”:
1. Odebranie zlecenia - Odebranie zlecenia na dostarczenie przesyłek z jednego
magazyny do drugiego.
2. Dostarczenie paczek - Przewóz paczek z jednego magazynu do drugiego.
3. Zgłoszenie utrudnień w dostawie - W Przypadku zaistnienia nieprzewidzianego
zdarzenia które może utrudnić lub opóźnić dostawę paczek Kierowca ma możliwość
poinformowania o tym swoich przełożonych.
Lista przypadków użycia dla “Klient”:
Zintegrowany Program Rozwoju Politechniki Lubelskiej
1. Przygotowanie paczki do nadania - zarejestrowanie nowej paczki w systemie oraz
pozyskanie etykiety z danymi paczki.
2. Rezygnacja z nadania paczki - możliwość zrezygnowania z nadania paczki gdy ta nie
została jeszcze włożona do paczkomatu.
3. Nadanie paczki - włożenie paczki z kodem QR do paczkomatu.
4. Odebranie paczki - wyjęcie paczki z paczkomatu za pomocą kodu QR
5. Śledzenie paczki - sprawdzanie stanu i położenia paczki
6. Archiwizacja paczki - Przeniesienie przez klienta w aplikacji mobilnej
odebranych/nadanych paczek do archiwum.
7. Przekierowanie paczki - zmiana adresu doręczenia paczki
8. Utworzenie konta - stworzenie nowego użytkownika w bazie danych
9. Edycja konta - usuwanie, zmienianie dodawanie danych odnośnie konta.
Lista przypadków użycia dla “Paczkomat”:
1. Otwieranie skrytek - otworzenie wybranych skrytek za pomocą systemu.
Lista przypadków użycia dla “System płatności”:
1. Płatność - przyjęcie i przetworzenie płatności za nadanie paczki a następnie określenie
czy płatność się powiodła.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
SCENARIUSZE PRZYPADKÓW UŻYCIA
S1. Utworzenie konta dla nowego pracownika
S1.1. Opis
Scenariusz przypadku użycia opisujący utworzenie konta w systemie wewnętrznym firmy dla
nowego pracownika.
 S1.2. Aktorzy
Administrator.
S1.3. Warunki początkowe
Administrator otrzymał dane pracownika.
S1.4. Warunki końcowe
Administrator wprowadził dane pracownika do systemu oraz przekazał mu hasło i login do
systemu.
S1.5. Przebieg główny
1. Administrator loguje się do systemu.
2. System wyświetla informację zleceniu dodania nowego pracownika do systemu.
3. Administrator rozpoczyna tworzenie konta dla pracownika.
4. System tworzy powiązanie danych pracownika z jego kontem.
5. Administrator nadaje odpowiednie uprawnienia dla konta pracownika.
6. System generuje login i hasło dla pracownika.
7. System przesyła dane uwierzytelniające na skrzynkę pocztową pracownika.
8. Administrator potwierdza utworzenie konta.
S1.6. Przebiegi alternatywne
PA.7. Pracownik nie podał adresu e-mail.
PA.7.1. System przesyła dane uwierzytelniające za pomocą wiadomości SMS na numer
telefoniczny podany przez pracownika.
PA.7.2. Powrót do punktu 8 przebiegu głównego.
S1.7. Sytuacje wyjątkowe
SW.1. Dane uwierzytelniające nie dotarły do pracownika.
Akcja: System generuje nowe dane uwierzytelniające i ponownie nadaje je do pracownika.
Jeżeli sytuacja powtórzy się kolejny raz system wysyła dane do pracownika innym sposobem.
SW.2. Dane uwierzytelniające wygasły.
Akcja: System generuje nowe dane uwierzytelniające i ponownie nadaje je do pracownika.
S1.8. Wymagania niefunkcjonalne
1. Dane uwierzytelniające wygenerowane przez system powinny być jednorazowe oraz
tracić ważność po upływie określonego czasu.
S1.9.Uwagi i pytania otwarte
Brak.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
S2. Dostarczenie paczek.
S2.1. Opis
Scenariusz przypadku użycia opisujący dostarczenia paczki do paczkomatu przez kuriera.
 S2.2. Aktorzy
Kurier.
S2.3. Warunki początkowe
Kurier odebrał paczki i dostał informacje gdzie ma je dostraczyć.
S2.4. Warunki końcowe
Kurier włożył paczki do odpowiedniego paczkomatu.
S2.5. Przebieg główny
1. Kurier odbiera paczkę z paczkomatu.
2. Zatwierdza w aplikacji odbiór paczek.
3. Wyrusza w kierunku paczkomatu docelowego.
4. Kurier za pomocą systemu otwiera odpowiednie skrytki w paczkomacie.
5. Kurier wkłada paczki do paczkomatu.
6. Zatwierdza w aplikacji włożenie paczek.
7. Automatycznie wysyłana jest wiadomość dla klienta z kodem QR do odbioru paczki.
S2.6. Przebiegi alternatywne
PA.1. Kurier nie może otworzyć paczkomatu.
PA.1.1. System przesyła kod zapasowy aby jednorazowo otworzyć skrytki w paczkomacie.
PA.1.2. Powrót do punktu 5 przebiegu głównego.
S2.7. Sytuacje wyjątkowe
SW.1. Paczka została uszkodzona w transporcie.
Akcja: Zgłaszamy w aplikacji zniszczenie paczki w transporcie i rejestrujemy dany kod paczki
jako ,,paczka uszkodzona”.
S2.8. Wymagania niefunkcjonalne
Dane uwierzytelniające wygenerowane przez system powinny być jednorazowe oraz tracić
ważność po upływie określonego czasu.
S2.9.Uwagi i pytania otwarte
Brak.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
S3. Rozpoczęcie pracy kuriera.
S3.1. Opis
Scenariusz przypadku rozpoczęcia pracy przez kuriera.
 S3.2. Aktorzy
Kurier.
S3.3. Warunki początkowe
Kurier zalogował się do aplikacji.
S3.4. Warunki końcowe
Kurier rozpoczyna szukanie przesyłek do przewozu.
S3.5. Przebieg główny
1. Kurier loguje się aplikacji.
2. Przypisuje do swojego konta numer auta jakie bierze.
3. Przypisuje do swojego konta numer identyfikatora jaki bierze.
4. Kurier wyszukuje paczkomaty, które mają paczki do odebrania.
5. System wyświetla listę paczkomatów z przesyłkami do odebrania.
6. Kurier wybiera paczkomat.
7. System zatwierdza wybór i zmienia status paczek które mają być odebrane.
S3.6. Przebiegi alternatywne
PA.6. Kierowca nie może się zalogować do aplikacji,
PA.6.1. System wysyła maila, na którym można zresetować hasło.
PA.6.2. Po zresetowaniu hasła kierowca musi ponownie podać wszystkie dane w celu
weryfikacji.
PA.6.3. Powrót do punktu 1 przebiegu głównego.
S3.7. Sytuacje wyjątkowe
SW.1. Kierowca jest nietrzeźwy.
Akcja: Wysyłamy do systemu dane odnośnie danego kierowcy i podejmujemy dalsze kroki w
sprawie jego pracy.
SW.2.Auto nie spełnia wymogów technicznych.
Akcja: System wyznacza nowe auto dla kierowcy. Niesprawne auto zostaje skierowane do
serwisu i jest niedostępne dla kierowców do momentu potwierdzenia jego działania.
S3.8. Wymagania niefunkcjonalne
Dane uwierzytelniające wygenerowane przez system powinny być jednorazowe oraz tracić
ważność po upływie określonego czasu.
S3.9.Uwagi i pytania otwarte
Brak.
S4. Zgłoszenie usterki towaru.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
S4.1. Opis
Scenariusz przypadku zgłaszania w systemie uszkodzonej paczki.
 S4.2. Aktorzy
Pracownik Magazynu.
S4.3. Warunki początkowe
Paczka dotarła do magazynu z paczkomatu lub z innego magazynu i jest widocznie
uszkodzona.
S4.4. Warunki końcowe
Pracownik magazynu pomyślnie zgłosił uszkodzenie paczki oraz przetransportował ją do
miejsca przeznaczonego na składowanie uszkodzonych paczek na terenie magazynu..
S4.5. Przebieg główny
1. Pracownik Magazynu skanuje kod QR paczki.
2. Skaner kodów QR z wyświetlaczem wyświetla informacje o paczce.
3. Pracownik Magazynu oznacza paczkę jako uszkodzoną w systemie informatycznym.
4. System wewnętrzny zapisuje informacje o uszkodzeniu paczki do bazy danych.
5. System wewnętrzny informuje Pracownika Magazynu o pomyślnym zgłoszeniu
uszkodzonej paczki.
S4.6. Przebiegi alternatywne
PA.1. Kod QR jest uszkodzony.
PA.1.1. Wybranie opcji o nieudanym skanowaniu na ekranie skanera kodów QR.
PA.1.1. Powiadamiany jest o tym szef zmiany i wykonywane są kroki mające na celu ustalenie
danych paczki.
PA.1.2. Drukowana jest nowa etykieta z kodem QR.
PA.1.3. Przejście do punktu 1. przebiegu głównego.
S4.7. Sytuacje wyjątkowe
SW.1. Szef zmiany nie jest w stanie ustalić danych paczki.
Akcja: Sytuacja zgłaszana jest do kierownictwa które kontaktuje się z klientem.
S4.8. Wymagania niefunkcjonalne
Brak.
S4.9.Uwagi i pytania otwarte
Brak.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
S5. Przygotowanie paczki do nadania.
S5.1. Opis
Scenariusz przypadku przygotowania paczki do nadania przez Klienta.
 S5.2. Aktorzy
Klient, System płatności.
S5.3. Warunki początkowe
Klient chce nadać paczkę.
S5.4. Warunki końcowe
Klient jest w posiadaniu etykiety z danymi paczki.
S5.5. Przebieg główny
1. Klient naciska przycisk nadania paczki.
2. System przesyła do klienta dostępne gabaryty i priorytety paczek.
3. System przenosi Klient do strony nadawania paczki.
4. Klient określa gabaryt i priorytet paczki.
5. Klient wpisuje dane odbiorcy.
6. Klient wybiera paczkomat nadania i odbioru.
7. System potwierdza możliwość nadania paczki w wybranym przez Klient punkcie.
8. System dodaje dane paczki do bazy danych.
9. System przenosi Klienta do strony z płatnością.
10. Klient realizuje płatność która zostaje przetworzona przez System Płatności.
11. System wyświetla Klientowi informację o przyjęciu zlecenia i przenosi Nadawcę do
widoku generacji etykiety.
12. Klient wybiera opcję generacji etykiety.
13. System wewnętrzny generuję dla klienta etykietę.
14. System przesyła do klienta wygenerowaną etykietę.
S5.6. Przebiegi alternatywne
PA.2. Klient nie posiada wymaganych uprawnień do zasobów
PA.2.1. Klient zostaje przeniesiony do ekranu logowania
PA.2.2. Klient loguje się
PA.2.3. System potwierdza autoryzację klienta i udostępnia klientowi listę dostępnych
gabarytów i priorytetów paczki.
PA2.4. Powrót do punktu 4 przebiegu głównego.
PA.6. Niemożliwe jest nadanie paczki z wybranego paczkomatu z powodu braku wolnych
skrytek.
PA.6.1. System informatyczny wyświetla informację o braku możliwości nadania paczki z
wybranego przez Klienta paczkomatu.
PA.6.2. System umożliwia Klientowi ponowne wybranie paczkomatu nadania i odbioru.
PA.6.3. Powrót do punktu 7.
S5.7. Sytuacje wyjątkowe
SW.1. Nie można było udostępnić gabarytów i priorytetów paczki z powodu nie znalezienia
określonych zasobów na serwerze.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Akcja: Klient dostaje informację o niepowodzeniu udostępnienia zasobów przez serwer i
zostaje przeniesiony do ekranu głównego.
SW.2. Płatność zakończona niepowodzeniem
Akcja: Klient dostaje informację o niepowodzeniu płatności i zostaje przeniesiony do ekranu
głównego. Nadanie paczki zostaje anulowane.
S5.8. Wymagania niefunkcjonalne
Brak.
S5.9.Uwagi i pytania otwarte
Brak.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
S6. Śledzenie paczki.
S6.1. Opis
Scenariusz przypadku śledzenia paczki przez Klient.
 S6.2. Aktorzy
Klient.
S6.3. Warunki początkowe
Klient chce śledzić paczkę.
S6.4. Warunki końcowe
Klient pomyślnie otworzył panel śledzenia paczki w aplikacji.
S6.5. Przebieg główny
1. Klient otwiera aplikację Express Paczka i loguje się.
2. Klient otwiera panel śledzenia paczek, następnie wybiera paczkę którą chce śledzić.
3. System informatyczny pobiera dane o paczce z bazy danych i wysyła je do Klienta.
4. Klient odbiera informacje o paczce.
S6.6. Przebiegi alternatywne
PA.3. W systemie informatycznym nie znajdują się informacje o obecnej lokalizacji paczki.
PA.3.1. Paczka nie została jeszcze zarejestrowana, wyświetlane są wstępne informacje.
PA.3.1. Powrót do punktu 4.
S6.7. Sytuacje wyjątkowe
SW.1. W aplikacji Express Paczka nie jest dostępna opcja wybrania nadanej przez nadawcę
paczki.
Akcja: Sytuacja zgłaszana jest do kierownictwa które próbuje ustalić przyczyny zaistniałego
błędu i podjąć próbę jego rozwiązania.
S6.8. Wymagania niefunkcjonalne
Brak.
S6.9.Uwagi i pytania otwarte
Brak.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
S7. Odebranie paczki.
S7.1. Opis
Scenariusz przypadku odebrania paczki przez Klienta.
 S7.2. Aktorzy
Klient, Paczkomat.
S7.3. Warunki początkowe
Klient dostał powiadomienie o możliwości odbioru przesyłki.
S7.4. Warunki końcowe
Klient odebrał przesyłkę.
S7.5. Przebieg główny
1. Klient otwiera aplikację.
2. Klient wybiera w aplikacji paczkę którą chce odebrać.
3. Aplikacja pobiera dane o paczce z bazy danych.
4. Klient naciska przycisk “Wyświetl kod QR”.
5. Aplikacja wyświetla kod QR odbioru paczki.
6. Klient skanuje kod QR w Paczkomacie.
7. Paczkomat otwiera skrytkę.
8. Klient wyjmuje paczkę z Paczkomatu i zamyka skrytkę.
9. System wyświetla ekran potwierdzenia odbioru paczki.
10. Klient potwierdza odebranie paczki.
11. System aktualizuje status paczki i datę odbioru.
S7.6. Przebiegi alternatywne
PA.3. Klient nie posiada wymaganych uprawnień do zasobu
PA.3.1. Klient zostaje przeniesiony do ekranu logowania
PA.3.2. Klient loguje się
PA.3.3. System potwierdza autoryzację klienta i udostępnia klientowi dane o wybranej paczce
PA.3.4. Powrót do punktu 4 przebiegu głównego.
PA.4. Klienta chce otworzyć skrytkę zdalnie.
PA.4.1. Klienta naciska przycisk “Otwórz zdalnie”
PA.4.2. Aplikacja pyta o zgodę na włączenie lokalizacji.
PA.4.3. Klienta potwierdza.
PA.4.4. Aplikacja sprawdza czy Klienta znajduje się w pobliżu Paczkomatu.
PA.4.5. Aplikacja wyświetla pytanie czy Klienta jest gotowy na otworzenie skrytki.
PA.4.6. Klient potwierdza.
PA.4.7. Powrót do punktu 7 przebiegu głównego.
PA.8. Klient zamknął skrytkę ale nie wyjął z niej paczki
PA.8.1. Aplikacja wyświetla ekran potwierdzenia odbioru paczki.
PA.8.2. Klient wybiera opcję “Otwórz jeszcze raz”.
PA.8.3. Powrót do punktu 4 przebiegu głównego.
S7.7. Sytuacje wyjątkowe
SW.1. Nie może znaleźć danych wybranej paczki.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Akcja: Klient dostaje informację o niepowodzeniu udostępnienia zasobów przez serwer i
zostaje przeniesiony do ekranu głównego.
SW.2. Zeskanowany kod QR został odrzucony przez paczkomat.
Akcja: Paczkomat wyświetla informację o odrzuceniu kodu QR. Klient może zgłosić problem z
otwarciem paczkomatu i zażądać wygenerowania nowego kodu QR.
SW.3. Przeterminowanie zgody na otwarcie skrytki zdalnie
Akcja: Aplikacja wyświetla klientowi informację o przeterminowaniu zgody na otwarcie
skrytki. Klient może ponowić próbę odebrania paczki.
SW.4. Klient nie potwierdził odebrania paczki.
Akcja: Odebranie paczki zostanie potwierdzone automatycznie po upływie 10 minut jeżeli
skrytka została zamknięta
S7.8. Wymagania niefunkcjonalne
1. Paczkomat powinien posiadać czytnik kodów QR.
2. Paczkomat powinien być w stanie wykryć czy skrytka jest otwarta.
3. W bazie danych powinny znajdować się współrzędne geograficzne paczkomatu.
S7.9.Uwagi i pytania otwarte
Brak.
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DIAGRAM PRZYPADKÓW UŻYCIA
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DIAGRAM KLAS
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DIAGRAMY SEKWENCJI
PRZYGOTOWANIE PACZKI DO NADANIA - KAROL HETMAN
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ODEBRANIE PACZKI - KAROL HETMAN
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DOSTARCZENIE PACZEK - MICHAŁ GRZESZUK
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ROZPOCZĘCIE PRACY KURIERA - MICHAŁ GRZESZUK
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ZGŁOSZENIE USTERKI TOWARU - MICHAŁ GOLUCH
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ŚLEDZENIE PACZKI - MICHAŁ GOLUCH
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DIAGRAMY AKTYWNOŚCI
PRZYGOTOWANIE PACZKI DO NADANIA - KAROL HETMAN
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ODEBRANIE PACZKI - KAROL HETMAN
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DOSTARCZENIE PACZEK - MICHAŁ GRZESZUK
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ROZPOCZĘCIE PRACY KURIERA - MICHAŁ GRZESZUK
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ZGŁOSZENIE USTERKI TOWARU - MICHAŁ GOLUCH
Zintegrowany Program Rozwoju Politechniki Lubelskiej
ŚLEDZENIE PACZKI - MICHAŁ GOLUCH
Zintegrowany Program Rozwoju Politechniki Lubelskiej
DIAGRAM ROZLOKOWANIA
Zintegrowany Program Rozwoju Politechniki Lubelskiej
Raport powstał podczas zajęć laboratoryjnych z przedmiotu
prowadzonego w ramach projektu
„Zintegrowany Program Rozwoju Politechniki Lubelskiej – część
druga”,
umowa nr POWR.03.05.00-00-Z060/18-00
w ramach Programu Operacyjnego Wiedza Edukacja Rozwój 2014-
2020
współfinansowanego ze środków Europejskiego Funduszu
Społecznego
