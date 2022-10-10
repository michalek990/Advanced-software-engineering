# Express Paczka

Express Paczka to aplikacja, która pozwala każdemu zostać dostawcą paczek. Nasza aplikacja
oferuję przewóz paczek na terenie całej Polski. Zatrudniamy i szkolimy kierowców. Aby
rozpocząć pracę w naszej firmie należy założyć konto w aplikacji, okazać potrzebne
dokumenty, przejść krótkie szkolenie i już można ruszać w trasę.
Wyróżniamy się szybkością dostarczania paczek. Nasi kurierzy jeżdżą 24 godziny na dobę.
Również bardzo przykładamy uwagę do jakości naszego transportu. Każda paczka
przewożona jest w bezpieczny sposób oraz dbamy o to aby nie została uszkodzona w
transporcie lub w trakcie kontaktu z paczkomatem.

---

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

Kierowcy wewnętrzni wożą paczki miedzy magazynami, zatrudniani są na pełen etat.
Paczki przewożone są w przypadku kiedy są przydzielone one do dostarczenia do innej
placówki. Kierowcy jeżdżą naszymi specjalnie oznaczonymi samochodami ciężarowymi.

# SPECYFIKACJA AKTORÓW
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

# HISTORYJKI UŻYTKOWNIKA
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
systemie
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
21. Jako “Kurier” chciałbym, aby system informatyczny automatycznie zmieniał status
paczki po jej włożeniu lub wyjęciu z paczkomatu.
22. Jako “Kurier” chciałbym, za pomocą systemu informatycznego sprawdzać o jakim
priorytecie jest dana paczka.
23. Jako “Kurier” chciałbym mieć możliwość zgłoszenia problemów z funkcjonowaniem
paczkomatu.

# WYMAGANIA FUNKCJONALNE
## W ramach projektowanego systemu, dla aktora „Kurier” przewidziano następującą funkcjonalność:
1. Logowanie do aplikacji - rozpoczęcie pracy i przydzielenie auta do kierowcy.
2. Wyszukiwanie punktów odbioru - szukanie przez kierowców zleceń do odbioru.
3. Odbieranie paczek - przesłanie przez system informatyczny do kierowcy informacji o
tym, który paczkomat zawiera paczki do odebrania.
4. Dostarczanie paczek - przesłanie przez system informatyczny do kierowcy informacji
o tym gdzie ma dostarczyć daną paczkę.
5. Zgłoszenie uszkodzenia towaru - przesłanie przez system informatyczny do
administratora informacji odnośnie uszkodzenia paczki
6. Zgłaszanie awarii paczkomatu - przesłanie do systemu informatycznego informacji o
uszkodzeniu lub awarii paczkomatu.


## W ramach projektowanego systemu, dla aktora „Pracownik magazynu” przewidziano następującą funkcjonalność:
1. Wyświetlanie danych o przesyłce - po zeskanowaniu kodu QR paczki wyświetlają się
informacje o paczce, między innymi o tym, gdzie trzeba przetransportować paczkę na
terenie magazynu.
2. Potwierdzenie odbioru przesyłki - po zeskanowaniu kodu QR paczki w systemie
powinna zostać zaktualizowana informacja o lokalizacji paczki tym samym
potwierdzając jej dotarcie do określonej sortowni.
3. Potwierdzenie nadania przesyłki - przesłanie do systemu informatycznego informacji
o miejscu do którego została nadana paczka


## W ramach projektowanego systemu, dla aktora “Klient” przewidziano następującą funkcjonalność:
1. Nadanie paczki - wykorzystanie systemu informatycznego do nadania paczki w
wybranym przez klienta paczkomacie.
2. Wybór priorytetu - wybór priorytetu z jakim ma być nadana paczka.
3. Śledzenie paczki - funkcjonalność umożliwiająca śledzenie aktualnego statusu i
lokalizacji przesyłki.
4. Przekierowanie - zmiana paczkomatu, do którego ma zostać doręczona paczka.
5. Odebranie paczki - wykorzystanie systemu informatycznego do odebrania paczki w
wybranym przez klienta paczkomacie
6. Ustawienie metody płatności - powiązanie karty bankowej z kontem klienta.
7. Wykonanie płatności - opłacenie przesyłki przez klienta.

## W ramach projektowanego systemu, dla aktora „Kierowca” przewidziano następującąfunkcjonalność:
1. Przyjęcie zlecenia - Przesłanie do systemu potwierdzenia o odebraniu zlecenia na przewóz przesyłek
2. Raport z przewozu - Złożenie raportu na temat dostarczonych paczek do magazynu
docelowego.
3. Dokumentacja - Przesyłanie przez system informatyczny faktur paliwowych.
4. Zgłoszenie uszkodzenia towaru - przesłanie przez system informatyczny informacji
odnośnie uszkodzenia paczki

## W ramach projektowanego systemu, dla aktora “Administrator” przewidziano następującą funkcjonalność:
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


# WYMAGANIA NIEFUNKCJONALNE
1. Jako serwer webowy system powinien wykorzystywać Apache HTTP Server.
2. System powinien wykorzystywać MySQL w roli systemu zarządzania bazami danych.
3. Jako język programowania po stronie serwera powinien być wykorzystany język PHP.
4. W przypadku aplikacji mobilnej na system android wykorzystywanym językiem
programowania powinna być Java.
5. W przypadku aplikacji mobilnej na system iOS wykorzystywanym językiem
programowania powinien być Swift
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

