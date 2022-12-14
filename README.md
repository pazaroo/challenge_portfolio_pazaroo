# challenge_portfolio_pazaroo

# **Task 1️⃣**

## Subtask 1

Kartkóweczka: 7/10 punktów

## Subtask 2

Stworzenie tego repozytorium, ELO! 💢💝💨💫 like a magic 🐇

## Subtask 3

Cześć!🐱‍👤
Mam na imię Kasia. Zdecydowałam się na challenge w dareIT, ponieważ szukam dla siebie innej ścieżki zawodowej, nowych możliwości ✨. Przez ostatnie lata pracowałam w słabo płatnej branży 💵😿, w bardzo wąskiej niszy 🔐, która mocno ograniczyła dalsze perspektywy 👁‍🙈. Cieszę się, że dzięki (mam nadzieję udanemu 🙏) przebranżowaniu odkryję dużo więcej możliwości rozwoju 🚀🙀. Myślę, że pomoc w postaci kursu będzie nieoceniona 🧡🧡🧡

## Subtask 4

Testowanie funkcjonalne aplikacji https://scouts-test.futbolkolektyw.pl/

Aplikacja służy do gromadzenia danych o zawodnikach piłki nożnej, aby móc selekcjonować zawodników.

### Funkcjonalności

* logowanie
* wylogowanie
* dodawania i edycja gracza 
* dodawanie i edycja meczu dla gracza
* dodawanie i edycja raportu meczu dla gracza, wraz z dodaniem wydarzeń w czasie w trakcie meczu, np. dodaniem dośrodkowania, etc.
* komunikat o niezapisanym meczu na stronie głównej

Wg mnie funkcjonalności mogłyby być lepiej zaprezentowane. Stronę ciężko nawigować, jest nieintuicyjna, np. po przejściu do wybranego gracza, otrzymujemy jego kartę oraz mecze, w których brał udział i szczegółowe raporty dla poszczególnych meczy, lecz nagłówki nie są wyróżnione pod głównym nagłówkiem, jakim jest imię i nazwisko gracza.

Minusem również jest to, że można gracza o takim samym imieniu i nazwisku dodawać wiele razy (nawet biorąc pod uwagę datę urodzenia) - w tym wypadku system mógłby pokazywać komunikat, że dodawany gracz jest już w bazie danych i czy może użytkownik właśnie jego szuka.

Podoba mi się opcja filtrowania - choć tutaj warto by było dodać opcję "wyczyść wszystkie filtry" i "zaznacz wszystkie filtry", np. gdy chcemy zaznaczyć tylko jeden, a następnie np. zwiększyć liczbę pokazywanych kolumn.

### Bugs

1. Aplikacja pozwoliła na dodanie gracza jeszcze nie urodzonego
https://drive.google.com/file/d/1hMidNPrD6b5Pqkn16rouKuyVOgSx5dIo/view?usp=share_link

2. Aplikacja pozwoliła na dodanie wagi gracza o wartości minusowej
https://drive.google.com/file/d/12XS8tkpyTPP3qWqb2Yv4jUB5osM_3gBB/view?usp=share_link

3. Aplikacja pozwoliła na dodanie wzrostu gracza o wartości minusowej
https://drive.google.com/file/d/1I_wOoV42G8Mvy8ajQYxtqOv3Go01SgZB/view?usp=share_link

4. Aplikacja pozwoliła na wpisanie numeru telefonu złożonego z liter, nie cyfr
https://drive.google.com/file/d/11WI5LQn1qw9RYSXVUCcAl2Q_Qb9ksuVe/view?usp=share_link

5. Aplikacja nie przenosi do niezapisanego/edytowanego meczu po kliknięciu w link
https://drive.google.com/file/d/1tC9KrVYTjPj8G-LIkPf0sE1UYCzVv_xU/view?usp=share_link
https://drive.google.com/file/d/1mdA6MPaBvDfVEqwkn3CtkYMeGkLeuvCS/view?usp=share_link

6. W widoku edycji gracza jedynie pole "Dominująca noga" ma w sobie placeholder - reszta pól wyświetla nagłowek mniejszą czcionką nad polem do uzupełnienia. Potrzeba zsynchronizowania tego widoku.
https://drive.google.com/file/d/16uGMTI6FjGtIlx9_h2Qmyblam_1QeMlL/view?usp=share_link

7. Nie ma możliwości otworzenia karty zawodnika bez przechodzenia bezpośrednio do jej edycji
https://drive.google.com/file/d/1h3RNbGElikegEe36ak6XALxvespD-BgY/view?usp=share_link

8. Sekcja link do YouTube pozwala na wstawienie dowolnego linku (aplikacja nie rejestruje czy link jest umieszczony na platformie youtube).
https://drive.google.com/file/d/1Wbj5qusbo2G38Hi64ttHA-btRwgJFzxx/view?usp=share_link

9. Aplikacja mimo pracy w języku polskim wyświetla niektóre sekcje wciąż w języku angielskim 
https://drive.google.com/file/d/1tgObWgRLe8sGHObvLtXMzwOMFO88HY__/view?usp=share_link

10. Pole w filtrach w obszarze wiek pozwala wpisać liczbę minusową, a także wprowadzić znaki literowe. Sugestia: wiek tylko w pełnych liczbach
https://drive.google.com/file/d/1CSkcylIQiOuoYV6UeUKHdO5MkM0EOTQ6/view?usp=share_link

11. Funkcja zawijania tekstu nie jest aktywna w tabeli widoku graczy - pole jest na tyle szerokie, na ile najdłuższa treść w danej kolumnie
https://drive.google.com/file/d/13LgZEDQVzJ6KelO3OaXIcFxK8tK97iUj/view?usp=share_link
https://drive.google.com/file/d/1XNqrSwpoLkPls-NNfZsgkuQ8aowWVx99/view?usp=share_link

12. Ani sekcja filtry, ani sekcja selekcji widocznych kolumn nie zapewnia filtrowania zawodników po dominującej nodze
https://drive.google.com/file/d/19iEOV6I8e08e8RqA6RVsgFjFJNay8_b2/view?usp=share_link
https://drive.google.com/file/d/1YlTzXCSOVHu4CoJurgGROZqPXVbR239k/view?usp=share_link

13. Pytanie do UI designera i developera: czy sekcja filtry i kolumny nie mogłyby mieć wspólnej przestrzeni, jeśli pełnią podobną funkcję? Lub alternatywnie: czy sekcja filtry nie powinna być rozszerzona o wszystkie pola w arkuszu, jakie można uzupełnić? 

14. Dla stworzenia przejrzystej i możliwej do filtrowania bazy danych, proponuję z podkreślonych pól uczynić drop-down menu, ponieważ w przeciwnym razie użytkownik może wypełnić pola na różnych arkuszach w różny sposób, np. "lewa obrona", "left-wing defence", "obrońca lewa strona"
https://drive.google.com/file/d/1eX9d-AxbHqMJozxE5X2zW_zc-615bA1E/view?usp=share_link

15. Brak widoczności w aplikacji kto utworzył kartę danego gracza ani kiedy. 
https://drive.google.com/file/d/1vqgC19Zi58xEwbzHrz05PleXxBNpNTBq/view?usp=share_link
(pytanie do developera i product ownera: czy logując się do portalu jestem w stanie zobaczyc tylko wprowadzonych przeze mnie graczy i mecze, czy widzę wszystkich, którzy zostali do bazy danych wprowadzeni?)

16. Części widoku edycji meczu dla danego gracza z polami opisanymi nagłówkami w języku angielskim przy wybranym języku na stronie polskim
https://drive.google.com/file/d/1ydn4ESgm_7B3o4SixbdnWi8pL_4tDYu8/view?usp=share_link
(pytanie do developera i product ownera: czym jest "Web match", "general", "recenzja" w tym widoku? Myślę, że może to być mylne dla użytkownika.

17. Przyciski edycji tekstu w raporcie po najechaniu na nie wyświetlają nazwy funkcji w języku angielskim w widoku strony polskim
https://drive.google.com/file/d/1Bku5ilHRiCDIzOJ4tSyw_rsLTytrMBTd/view?usp=share_link

18. W widoku dodawania meczu aplikacja pozwoliła na dodanie minusowego czasu gry, minusowego unmeru zawodnika, a także daty, która jeszcze nie nadeszła
https://drive.google.com/file/d/1YoxjjvC14yNkNRliDHAALgQQ8T-WS0Kp/view?usp=share_link

19. Aplikacja pozwoliła na dodanie większej niż dwie połowy meczu
https://drive.google.com/file/d/16sox-dENeu1j5Zl-sEgU8BlIAvIh4pXv/view?usp=share_link

20. Jaką logikę ma ta lista? Gracze nie wydają się być ułożeni zgodnie z żadną logiką (imię, nazwisko, mecze, raortu, rezenzja). Propozycja: można dodać funkcjonalność "sortuj po" do każdej z kolumn.
https://drive.google.com/file/d/1NpU0EleqWBP4aoTPxDCBdZAGfQnATacp/view?usp=share_link

### Validations

1. Aplikacja działa prawidłowo, nie pozwalając na wprowadzenie liczba zdobytych goli w liczbie dziesiętnej
https://drive.google.com/file/d/1dX7e-FzNM_gJ3oi5m47-AjRbZlt_QaDF/view?usp=share_link

2. Aplikacja działa prawidłowo, nie pozwalając na wprowadzenie liczby zdobytych goli mniejszych od zera
https://drive.google.com/file/d/1pKExXmf3sSXCa4vx_v0wDhM223Fs5Vdp/view?usp=share_link

3. Aplikacja działa z dobrymi wynikami na poziomie ładowania widoku eydcji gracza
https://drive.google.com/file/d/1quMftoXVYaRzfrX6ykalOT6UlFfd0Vtr/view?usp=share_link

4. Aplikacja po kliknięciu łącza przenosi na stronę logowania do aplikacji Slack
https://drive.google.com/file/d/1BoxIY2IqkSRsy4EoqP5Q6NSGz4wNGHcd/view?usp=share_link


### Design

1. Aplikacja po przejściu na widok mobilny i przejsciu do sekcji gracze pokazuje ich w formie listy, a nie kart, jak w przypadku wersji webowej, ale poszczególni gracze zlewają się ze sobą wizualnie ze względu na brak przerwy/grubszej linii lub innego elementu wizualnego
https://drive.google.com/file/d/189qFVzrEOAXdYHYCuqeTGQyq0Ba1avAM/view?usp=share_link

2. Na widoku edycji raportu meczowego, szerokość strony się zwiększa względem widoku w reszcie aplikacji
Widok w edycji raportu
https://drive.google.com/file/d/1eilmYO2IFR45Wy1xdbF13BpxW8xWurhZ/view?usp=share_link
Widok np. edycji meczu
https://drive.google.com/file/d/1fGbyRaRdIYNYvLk_xj1gDWxtNlU4KfCU/view?usp=share_link

3. Pytanie do designera/developera: czy nie miałoby sensu osadzenie pliku video z youtube w zakładce zawodnika, zamiast tworzenia miejsca dla wstawienia linku
https://drive.google.com/file/d/1x7c1cUq2N13m3z3LTOSd5Jjxc3pQuoBx/view?usp=share_link

4. Sugestia: dla lepszej, bardziej intuicyjnej obsługi aplikacji przenieść opcję dodawania z dość niecharakterystycznej sekcji "linki pomocnicze" do głównego menu po lewej stronie jako button
https://drive.google.com/file/d/1h9nrp2Y7aClKMFR_l6CB-fr1gKRkB9B8/view?usp=share_link

5. Wyalignować linie pól w sekcji filtry (w tym momencie znajdują się na różnych poziomach)
https://drive.google.com/file/d/1DhTRDhbDDenS1ikKbY2gNBdhTlcMKWIZ/view?usp=share_link

6. Ikony rozciągnięte nieproporcjonalnie w widoku tworzenia meczu. Boisko nie jest również w dobrych proporcjach do tych, które grafika przedstawia (centralny okrąg nie jest okręgiem, a elipsą).
https://drive.google.com/file/d/1qySSzH7bh9QTklBH7aX9UDPr7v5LX66U/view?usp=share_link

7. Narzędzia w edycji tworzenia meczu nie są intuicyjne i po zawiśnięciu nad przyciskiem (na screeshocie np 3 przycisk) nie pokazują się opisy funkcji. Pytanie do UI designera: może warto dodać?
https://drive.google.com/file/d/1lIezFZNrPYeopXx7wdigss84N6vZbyqr/view?usp=share_link

# **Task 2️⃣**

## Subtask 1

https://drive.google.com/drive/u/1/folders/1afRuVs8CiPq7uCGREQUOaVBgGJpt1Nir

## Subtask 2

https://drive.google.com/drive/u/1/folders/1DzV8xUE1ynFZjwz8P7EdWWuC3lLCjKfu

## Subtask 3️

_Po co piszemy test case’y?_

Przypadki testowe piszemy, aby udokumentować w przejrzysty sposób różne możliwości obsłużenia modułów w ramach danej aplikacji. Dobre pokrycie przypadkami testowymi oprogramowania daje nam pewność podczas testów, że nie pominęliśmy żadnej ważnej funkcjonalności. Pisanie przypadków testowych i zbieranie ich w scenariusze pozwala na usystematyzowanie pracy i uniknięcia zatracenia się w „wirze testowania” eksploracyjnego i błądzenia zespołu. Przypadki testowe gwarantują również możliwość powtarzalności testów i pracy w regresji.

# **Task 3️⃣**

## Subtask 1 & Subtask 2

_stworzenie formatki 📃 oraz przejście przez wcześniej utworzone przypadki testowe ✨ i zaraportowanie błędów 🐞_

https://drive.google.com/drive/u/1/folders/12AQkwclIYLCbnsqnYhmLkkmO63ZsaERU

## Subtask 3

_raport z wykonanych testów_ 👉 https://docs.google.com/presentation/d/1wVLtSimthwi6erCV-5VIrOsuGQK_5rt0t_2MSGiKgXE/edit?usp=share_link

 ![Manual testing of Panel Skautingowy report DareIT](https://user-images.githubusercontent.com/116814963/202041783-6af763d0-c2ab-4945-81cc-a75fd6a31450.jpg)

![Manual testing of Panel Skautingowy report DareIT](https://user-images.githubusercontent.com/116814963/202041808-f24e607b-bf8f-4ab7-80ec-228930334ff0.png)

![Manual testing of Panel Skautingowy report DareIT (1)](https://user-images.githubusercontent.com/116814963/202041847-204bf9ae-8b27-49af-92eb-2ab2bf3219f2.png)

![Manual testing of Panel Skautingowy report DareIT (2)](https://user-images.githubusercontent.com/116814963/202041865-1d761d29-d4fd-450a-b1a1-3e2a3e2e7b5e.png)

![Manual testing of Panel Skautingowy report DareIT (3)](https://user-images.githubusercontent.com/116814963/202041891-2f997c35-0ab7-4bb9-bfeb-190efbd1bad4.png)

![Manual testing of Panel Skautingowy report DareIT (4)](https://user-images.githubusercontent.com/116814963/202041905-22473007-d2df-4515-a5fc-4105310eaedf.png)

# **Task 4️⃣**

## Subtask 1 i 2

_Utworzenie formatki oraz testowanie eksploracyjne i raportowanie błędów_

Pełen raport pod linkiem:📃💡🔍👉 https://drive.google.com/drive/u/0/folders/1ScqRn0PHZLClMj_OXwfF_aiC7z4lp2r2 👈👌

![Bug report Focusly](https://user-images.githubusercontent.com/116814963/203171727-18575706-6cf1-4ed4-a721-b2986e13ce05.png)

![Bug report Focusly (1)](https://user-images.githubusercontent.com/116814963/203171759-407892bf-d953-4a0d-adab-ede369a48451.png)

![Bug report Focusly (2)](https://user-images.githubusercontent.com/116814963/203171772-d0d65f85-c8c7-4b95-b8b7-6279eec403fb.png)

![Bug report Focusly (3)](https://user-images.githubusercontent.com/116814963/203171808-f9d063c8-6261-49f0-b48e-b5fd7e9ab965.png)

![Bug report Focusly (4)](https://user-images.githubusercontent.com/116814963/203171820-fc61597d-6645-4bdd-8cca-d3c3fd55f4ca.png)

![Bug report Focusly (5)](https://user-images.githubusercontent.com/116814963/203171834-db9f2ad5-235a-46f0-9d73-cae4ec6e0a14.png)

## Subtask 3

_1. Do czego służy ta aplikacja? Jaki jest cel tej aplikacji❔_ 

Aplikacja pomaga w zachowaniu zdrowia psychicznego i fizycznego. Oferuje medytacje, podcasty nt. zdrowia psychicznego, radzenia sobie ze stresem, oddechu, swiadomosci (mindfulness), zarzadzania emocjami i relacjami. Przy jej pomocy mozna wykonywac prowadzone cwiczenia oddechowe czy odsluchac relaksujacej muzyki. 

_2. Kto ma być użytkownikiem końcowym aplikacji❔_

Użytkownikiem końcowym jest osoba swiadoma wagi zdrowia psychicznego we wspolczesnym swiecie, szukajaca sposobu na wdrozenie nawykow na co dzien, byc moze laik, ktory jest nowy w swiecie medytacji, etc. Jest to osoba, ktora jest zdigitalizowana, szuka odpowiedzi na problemy za pomoca nowych technologii. Jest to osoba, ktora chce moc w kazdym momencie dnia zatroszczyc sie o siebie i by aplikacja byla motywatorem zmian i sposobem na podtrzymanie ich. Dzieki aplikacji dokonanie zmian jest latwiejsze.

_3. Czy według Ciebie aplikacja jest user friendly❔ _

Aplikacja jest user friendly. Ma prosta i przejrzysta nawigacje. Rozpoznanie struktury aplikacji nie zajmuje wiele czasu, przyciski sa umieszczone w dobrych miejscach. Jednym z mankamentow jest bug, ktory uniemozliwia korzystanie z natywnych przyciskow nawigacji w Android oraz nawigacja na karuzelach i miedzy tabami, ktore to nakladaja sie na siebie. Sa to rzeczy irytujace z punktu widzenia uzytkownika, ktore na pewno powinny zostac naprawione. Z potrzebnymi zmianami sama chetnie uzywalabym aplikacji.

_4. Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność❔_

Umiescilabym na zakladce strona glowna wyszukiwarke - w tym momencie trzeba pamietac, ze znajduje sie ona w zakladce "Odkrywaj". Wg mnie wazne jest tez, aby aplikacja z medytacjami i muzyka relaksacyjna miala latwo dostepna biblioteke - w tym wypadku brakuje dedykowanego miejsca. Zamiast tego, do sekcji "Ulubione praktyki" dostaniemy sie z poziomu profilu (nieintuicyjne). Polubione materialy pokazuja sie w formie jednej listy bez rozroznienia czy jest to podcast, medytacja czy innego rodzaju aktywnosc. Wprowadzilabym kategorie materialow do odsluchania w czasie pojscia spac (np. white noise, nagranie szumiacego lasu 8 h, etc.). Mysle, ze warto by bylo dodac aspekt spolecznosciowy - np. opcje polecenia danego materialu znajomemu.

_5. Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej❔_

Aplikacja natywna ze wzgledu na brak nawigacji myszka odznacza sie duza wrazliwoscia na zle ulozone przyciski, nieodpowiedni ich rozmiar (zbyt male). Trzeba brac pod uwage dostepnosc przyciskow dla kciuka. Mysle, ze ze wgledu na duza konkurencje podobnych aplikacji na rynku, decyzja potencjalnego uzytkownika o tym czy z danej aplikacji nadal korzystac czy przerzucic sie na inna jest szybka. Testowanie aplikacji natywnej bierze mocno pod uwage powiazanie z aspektem sprzetowym (zuzycie baterii, dzialanie na poszczegolnych wersjach OS, roznych rozdzielczosciach i wielkosciach ekranu, etc.)

# **Task 5️⃣**

## Subtask 1 - Krótki kurs podstaw SQL

Wykorzystałam następujące linki do nauki 📚

👍 https://www.w3schools.com/sql/

👍 https://www.cognity.pl/top-50-zapytan-sql,blog,390.html

👍 https://bulldogjob.pl/readme/dlaczego-warto-uczyc-sie-sql

👍 https://epicdigitalguy.com/blog/2020/07/24/mysql-cheat-sheet/

👍 https://www.kursysql.pl/sql-w-120-minut/

👍 https://tomaszkenig.pl/kurs-sql-server/operatory-logiczne-w-sql-server/

A nauczyłam się tego:

`select  from table_name`
do wyświetlenia/wybrania wszystkich rekordów dla danej tabeli

`select column_name from table_name`
do wybrania wszystkich rekordów z kolumny o danej nazwie dla danej tabeli

`select distinct column_name from table_name`
do wybrania różnych rekordów w danej kolumnie w danej tabeli

`select  from table_name where column_name='nazwa'`
do wybrania wszystkich rekordów o określonej nazwie z danej kolumny w danej tabeli

`select  from table_name where not column_name='nazwa'`
do wybrania wszystkich rekordów poza tymi o określonej nazwie z danej kolumny w danej tabeli

`select  from table_name where column_name=1`
do wybrania wszystkich rekordów danej kolumny w danej tabeli o wartości 1

`select  from table_name where column_name=[1-90]`
do wybrania wszystkich rekordów danej kolumny w danej tabeli o wartości między 1 a 90

`select  from table_name where column_name='%t`
do wybrania wszystkich rekordów danej kolumny w danej tabeli kończących się na t

`select  from table_name where column_name='t%`
do wybrania wszystkich rekordów danej kolumny w danej tabeli zaczynających się na t

`select  from table_name where column_name='t%z`
do wybrania wszystkich rekordów danej kolumny w danej tabeli zaczynających się na t i kończących się na z

`select  from table_name where column_name='____`
do wybrania wszystkich rekordów danej kolumny w danej tabeli o 4 znakach literowych

`select  from table_name where column_name='gr[!a-k]%`
do wybrania wszystkich rekordów danej kolumny w danej tabeli zaczynającyh się od gr, w których następnym znakiem nie jest żadna litera z zakresu a-k, oraz która po tym może mieć dowolną liczbę znaków (włączając w to brak kolejnych znaków)

`select column_nam1e, column_name2, column_name3 from table_name order by column_name='gr[!a-k]%`
do wybrania wszystkich rekordów danej kolumny w danej tabeli zaczynającyh się od gr, w których następnym znakiem nie jest żadna litera z zakresu a-k, oraz która po tym może mieć dowolną liczbę znaków (włączając w to brak kolejnych znaków)

Poza tym przećwiczyłam następujące komendy:

- insert into * values
- is null 
- is not null
- update * set
- delete from * where
- select min()
- select max()
- select * from * where * in ('x', 'y', 'z')
- select * from * where * between 1 and 9
- select * from * where not * between 'Basia' and 'Kasia'
- select * as * 

## Subtask 2 - Konfiguracja środowiska i wgranie bazy danych - DONE! ✔

## Subtask 3 - Kilka zadań na rozgrzewkę, _czyli sprawdzenie wiedzy w praktyce!_

**_1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname._**

SELECT * FROM `actors`
order by surname ASC

![image](https://user-images.githubusercontent.com/116814963/204662690-8d25c161-41db-4220-af20-fa30ae7aa535.png)

**_2. Wyświetl film, który powstał w 2019 roku._**

SELECT * FROM `movies`
where year_of_production=2019

![image](https://user-images.githubusercontent.com/116814963/204663277-47c90621-e560-44da-a9bd-fc6277fd5566.png)

**_3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem._**

SELECT * FROM `movies`
where year_of_production between 1900 and 1999

![image](https://user-images.githubusercontent.com/116814963/204663587-850adaae-ce55-47af-ab88-a7ae9ef562d7.png)

**_4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$._**

SELECT title, price FROM `movies`
WHERE price < 7

![image](https://user-images.githubusercontent.com/116814963/204664469-e03c633b-aef4-4916-bf9a-6d6981217896.png)

**_5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN._**

SELECT * FROM `actors` WHERE actor_id > 3 and actor_id < 8

![image](https://user-images.githubusercontent.com/116814963/204668905-c4c23d9a-d7ce-425f-843b-f628971ed477.png)

**_6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny._**

SELECT * FROM `customers` WHERE customer_id=2 or customer_id=4 or customer_id=6

![image](https://user-images.githubusercontent.com/116814963/204666742-44271320-9724-4ced-b597-5590f9643386.png)

**_7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN._**

SELECT * FROM `customers` WHERE customer_id in (1,3,5)

![image](https://user-images.githubusercontent.com/116814963/204667030-99d957b8-0e56-4fac-8f51-cae85a89aafe.png)

**_8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”._**

SELECT * FROM `actors` WHERE name like 'an%'

![image](https://user-images.githubusercontent.com/116814963/204667439-120b797d-4f85-4521-82f1-a9f566175a8d.png)

**_9. Wyświetl dane klienta, który nie ma podanego adresu email._**

SELECT * FROM `customers` WHERE email is null

![image](https://user-images.githubusercontent.com/116814963/204667640-46f53d59-6114-4d2d-83c4-c9d8ce594f0d.png)

**_10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id._**

SELECT * FROM `movies` WHERE price > 9 and movie_id between 2 and 8

![image](https://user-images.githubusercontent.com/116814963/204667828-e4ac745b-ea33-4092-b33a-aa05108fa9bb.png)

💖💥🙏🐇

# **Task 6️⃣**

## Subtask 1 - Krótki kurs podstaw SQL - ciąg dalszy

**_11. Skoryguj nazwisko Ani Muler na Muler._**

update customers
set surname = 'miler'
where name = 'ania'

![image](https://user-images.githubusercontent.com/116814963/205995451-a02cdaa6-c7e9-4f47-b9f0-d4cd4dbc8511.png)

**_12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej._**

select sale.customer_id, sale.movie_id, customers.email, customers.name
from customers
inner join sale on customers.customer_id=sale.customer_id
where movie_id=4

![image](https://user-images.githubusercontent.com/116814963/206018304-37dc44aa-7a37-4d54-afe8-2a73c386f77d.png)

**13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com**

update customers
set email='pati@mail.com' where name='Patrycja'

![image](https://user-images.githubusercontent.com/116814963/206019283-899a1189-d440-4205-9164-1c35080e2246.png)

**14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).**

SELECT sale.customer_id, sale.movie_id, movies.title, customers.name, customers.surname
from sale
inner join movies
on sale.movie_id=movies.movie_id
inner join customers
on sale.customer_id=customers.customer_id

![image](https://user-images.githubusercontent.com/116814963/206021898-a8fac194-000a-4920-8f4d-4f5a2a4485b0.png)

**15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag**

alter table customers
add pseudonym char(3)

![image](https://user-images.githubusercontent.com/116814963/206040988-3d88941f-2982-40b4-bcab-ec487c890212.png)



**16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.**

SELECT DISTINCT movies.title FROM movies INNER JOIN sale ON sale.movie_id = movies.movie_id;

![image](https://user-images.githubusercontent.com/116814963/206031772-f3736748-fd74-4418-a94d-731d1a4b66a0.png)

**17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)**

SELECT name FROM actors
UNION
SELECT name FROM customers
order by name asc

![image](https://user-images.githubusercontent.com/116814963/206032500-80c840db-d915-41ca-8967-695ab2c30f73.png)

** 18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie). **

UPDATE movies
set price = price + 2.5
WHERE movies.year_of_production > 2000

![image](https://user-images.githubusercontent.com/116814963/206033718-60029a86-ce44-4690-be95-0abb7a5e0a52.png)

**19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał**

SELECT actors.name, actors.surname, movies.title
from actors
inner join cast
on actors.actor_id=cast.actor_id
inner join movies
on cast.movie_id=movies.movie_id
where actors.actor_id=4

![image](https://user-images.githubusercontent.com/116814963/206034930-b3f7d4c4-b928-468e-9d69-a63ef3aa58a8.png)

**20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa**

