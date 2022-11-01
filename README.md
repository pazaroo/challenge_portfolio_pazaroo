# challenge_portfolio_pazaroo

# **Task 1**

## Subtask 1

7/10 punktów

## Subtask 3

Cześć! Mam na imię Kasia. Zdecydowałam się na challenge w dareIT, bo szukam dla siebie innej ścieżki zawodowej, nowych możliwości. Przez ostatnie lata pracowałam w słabo płatnej branży, w bardzo wąskiej niszy, która mocno ograniczyła dalsze perspektywy. Cieszę się, że dzięki (mam nadzieję udanemu) przebranżowaniu odkryję dużo więcej możliwości rozwoju. Myślę, że pomoc w postaci kursu będzie nieoceniona.

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
![image](https://user-images.githubusercontent.com/116814963/198838548-0be158e0-4f76-4da1-a193-c302340ddd78.png)

Wg mnie funkcjonalności mogłyby być lepiej zaprezentowane. Stronę ciężko nawigować, jest nieintuicyjna, np. po przejściu do wybranego gracza, otrzymujemy jego kartę oraz mecze, w których brał udział i szczegółowe raporty dla poszczególnych meczy, lecz nagłówki nie są wyróżnione pod głównym nagłówkiem, jakim jest imię i nazwisko gracza.

![image](https://user-images.githubusercontent.com/116814963/198841454-8ddd2f7e-eec9-4499-b5e9-2fb2fdbf6b73.png)

Minusem również jest to, że można gracza o takim samym imieniu i nazwisku dodawać wiele razy (nawet biorąc pod uwagę datę urodzenia) - w tym wypadku system mógłby pokazywać komunikat, że dodawany gracz jest już w bazie danych i czy może użytkownik właśnie jego szuka.

Podoba mi się opcja filtrowania - choć tutaj warto by było dodać opcję "wyczyść wszystkie filtry" i "zaznacz wszystkie filtry", np. gdy chcemy zaznaczyć tylko jeden, a następnie np. zwiększyć liczbę pokazywanych kolumn.

### Bugs

1. Aplikacja pozwoliła na dodanie gracza jeszcze nie urodzonego

![image](https://user-images.githubusercontent.com/116814963/198836139-a6e99552-6862-4dc7-8c57-29d0f649fd27.png)

2. Aplikacja pozwoliła na dodanie wagi gracza o wartości minusowej

![image](https://user-images.githubusercontent.com/116814963/198837077-352e6edd-48c3-4d38-b051-909a2557a51d.png)

3. Aplikacja pozwoliła na dodanie wzrostu gracza o wartości minusowej

![image](https://user-images.githubusercontent.com/116814963/198838100-1df7829b-5588-4f6d-aa97-e43cd66391c8.png)

4. Aplikacja pozwoliła na wpisanie numeru telefonu złożonego z liter, nie cyfr

![image](https://user-images.githubusercontent.com/116814963/198837881-70e90c7d-a812-421f-a56a-eb974bdc97f0.png)

5. Aplikacja nie przenosi do niezapisanego/edytowanego meczu po kliknięciu w link

![image](https://user-images.githubusercontent.com/116814963/198838723-3fbab763-f452-495b-b93b-474ee4ebfa67.png)
![image](https://user-images.githubusercontent.com/116814963/198838783-18b1a7ae-5ed8-4061-bc35-6fc76ded465a.png)

6. W widoku edycji gracza jedynie pole "Dominująca noga" ma w sobie placeholder - reszta pól wyświetla nagłowek mniejszą czcionką nad polem do uzupełnienia. Potrzeba zsynchronizowania tego widoku.

![image](https://user-images.githubusercontent.com/116814963/199271112-9ec234cf-0d07-4fb2-8963-b4cab0e8e025.png)

7. Nie ma możliwości otworzenia karty zawodnika bez przechodzenia bezpośrednio do jej edycji

![2022-11-01_16h29_20](https://user-images.githubusercontent.com/116814963/199272513-63f1f335-b09e-46c9-aa6a-6f63095a7f31.gif)

8. Sekcja link do YouTube pozwala na wstawienie dowolnego linku (aplikacja nie rejestruje czy link jest umieszczony na platformie youtube).

![image](https://user-images.githubusercontent.com/116814963/199272963-493f0da5-ca18-4b86-8ca4-f650c2547491.png)

9. Aplikacja mimo pracy w języku polskim wyświetla niektóre sekcje wciąż w języku angielskim 

![image](https://user-images.githubusercontent.com/116814963/199276245-27415068-e8f9-4e6c-9ed9-8f8c9056c25d.png)

10. Pole w filtrach w obszarze wiek pozwala wpisać liczbę minusową, a także wprowadzić znaki literowe. Sugestia: wiek tylko w pełnych liczbach

![image](https://user-images.githubusercontent.com/116814963/199276245-27415068-e8f9-4e6c-9ed9-8f8c9056c25d.png)

11. Funkcja zawijania tekstu nie jest aktywna w tabeli widoku graczy - pole jest na tyle szerokie, na ile najdłuższa treść w danej kolumnie

![image](https://user-images.githubusercontent.com/116814963/199276889-5e364127-90df-4a7c-a4d9-cd05753d73fb.png)

![2022-11-01_16h51_05](https://user-images.githubusercontent.com/116814963/199277660-bcc2d311-60c9-4881-8d83-d92644ad0e25.gif)

12. Ani sekcja filtry, ani sekcja selekcji widocznych kolumn nie zapewnia filtrowania zawodników po dominującej nodze

![image](https://user-images.githubusercontent.com/116814963/199278483-0d61b8d0-c769-4f96-84c3-29719eb89b5b.png)

![image](https://user-images.githubusercontent.com/116814963/199278521-0f0e29b6-8458-4ac6-a663-579211bb929c.png)

13. Pytanie do UI designera i developera: czy sekcja filtry i kolumny nie mogłyby mieć wspólnej przestrzeni, jeśli pełnią podobną funkcję? Lub alternatywnie: czy sekcja filtry nie powinna być rozszerzona o wszystkie pola w arkuszu, jakie można uzupełnić? 

14. Dla stworzenia przejrzystej i możliwej do filtrowania bazy danych, proponuję z podkreślonych pól uczynić drop-down menu, ponieważ w przeciwnym razie użytkownik może wypełnić pola na różnych arkuszach w różny sposób, np. "lewa obrona", "left-wing defence", "obrońca lewa strona"

![image](https://user-images.githubusercontent.com/116814963/199281054-5c66445d-9632-4426-a78a-ee7823fead60.png)

15. Brak widoczności w aplikacji kto utworzył kartę danego gracza ani kiedy. 

![image](https://user-images.githubusercontent.com/116814963/199281332-71aa6c65-7684-4ee9-8f6e-966300004f9f.png)

(pytanie do developera i product ownera: czy logując się do portalu jestem w stanie zobaczyc tylko wprowadzonych przeze mnie graczy i mecze, czy widzę wszystkich, którzy zostali do bazy danych wprowadzeni?)

16. Części widoku edycji meczu dla danego gracza z polami opisanymi nagłówkami w języku angielskim przy wybranym języku na stronie polskim

![image](https://user-images.githubusercontent.com/116814963/199282410-8c75f7bf-f802-400d-a478-166f1c24d5b3.png)

(pytanie do developera i product ownera: czym jest "Web match", "general", "recenzja" w tym widoku? Myślę, że może to być mylne dla użytkownika.

17. Przyciski edycji tekstu w raporcie po najechaniu na nie wyświetlają nazwy funkcji w języku angielskim w widoku strony polskim

![image](https://user-images.githubusercontent.com/116814963/199283595-db4ca176-9db2-477f-bab9-e645428e6c18.png)

18. W widoku dodawania meczu aplikacja pozwoliła na dodanie minusowego czasu gry, minusowego unmeru zawodnika, a także daty, która jeszcze nie nadeszła

![image](https://user-images.githubusercontent.com/116814963/199284423-d52845d9-a6b4-40b0-9fbd-763348378821.png)

19. Aplikacja pozwoliła na dodanie większej niż dwie połowy meczu

![image](https://user-images.githubusercontent.com/116814963/199286130-72ab7888-7202-4633-910b-0b948b9ff449.png)

20. Jaką logikę ma ta lista? Gracze nie wydają się być ułożeni zgodnie z żadną logiką (imię, nazwisko, mecze, raortu, rezenzja). Propozycja: można dodać funkcjonalność "sortuj po" do każdej z kolumn.
21. 
![image](https://user-images.githubusercontent.com/116814963/199289074-a393099c-b5fa-4a40-91e0-f10cdd0813cd.png)


### Validations

1. Aplikacja działa prawidłowo, nie pozwalając na wprowadzenie liczba zdobytych goli w liczbie dziesiętnej
![image](https://user-images.githubusercontent.com/116814963/198836764-a0556e58-ce8f-4d76-ac67-7a1cbfab5bee.png)

2. Aplikacja działa prawidłowo, nie pozwalając na wprowadzenie liczby zdobytych goli mniejszych od zera
![image](https://user-images.githubusercontent.com/116814963/198841931-d1f41ad1-8475-47e8-a488-690768330954.png)

3. Aplikacja działa z dobrymi wynikami na poziomie ładowania widoku eydcji gracza
 ![image](https://user-images.githubusercontent.com/116814963/198840860-0d6702f7-5eb8-4a16-bd17-39bc9a610383.png)
 
4. Aplikacja po kliknięciu łącza przenosi na stronę logowania do aplikacji Slack

![image](https://user-images.githubusercontent.com/116814963/199274463-91eb5ad9-6e96-4659-8327-3de958a9ab7c.png)


### Design

1. Aplikacja po przejściu na widok mobilny i przejsciu do sekcji gracze pokazuje ich w formie listy, a nie kart, jak w przypadku wersji webowej, ale poszczególni gracze zlewają się ze sobą wizualnie ze względu na brak przerwy/grubszej linii lub innego elementu wizualnego
![image](https://user-images.githubusercontent.com/116814963/198839023-40d43581-5642-4b3d-b5e4-0e6fd90f44d8.png)

2. Na widoku edycji raportu meczowego, szerokość strony się zwiększa względem widoku w reszcie aplikacji

Widok w edycji raportu
![image](https://user-images.githubusercontent.com/116814963/198841050-986d7468-db95-44ed-8517-5ad9e61d29ca.png)

Widok np. edycji meczu
![image](https://user-images.githubusercontent.com/116814963/198841102-fb509f37-8c6c-4798-98b3-5b868789f8d7.png)

3. Pytanie do designera/developera: czy nie miałoby sensu osadzenie pliku video z youtube w zakładce zawodnika, zamiast tworzenia miejsca dla wstawienia linku

![image](https://user-images.githubusercontent.com/116814963/199273220-4e32554f-b803-40ba-9d88-463f0eed7ac9.png)

4. Sugestia: dla lepszej, bardziej intuicyjnej obsługi aplikacji przenieść opcję dodawania z dość niecharakterystycznej sekcji "linki pomocnicze" do głównego menu po lewej stronie jako button

![image](https://user-images.githubusercontent.com/116814963/199274924-2b3f98d4-4b74-4899-9b3e-6dccfdd6daf2.png)

5. Wyalignować linie pól w sekcji filtry (w tym momencie znajdują się na różnych poziomach)

![image](https://user-images.githubusercontent.com/116814963/199289466-fb219c87-5b69-45c4-962b-19687acc61e5.png)

6. Ikony rozciągnięte nieproporcjonalnie w widoku tworzenia meczu. Boisko nie jest również w dobrych proporcjach do tych, które grafika przedstawia (centralny okrąg nie jest okręgiem, a elipsą).

![image](https://user-images.githubusercontent.com/116814963/199285091-fcaff373-4209-4896-8534-72d70ebdbb25.png)

7. Narzędzia w edycji tworzenia meczu nie są intuicyjne i po zawiśnięciu nad przyciskiem (na screeshocie np 3 przycisk) nie pokazują się opisy funkcji. Pytanie do UI designera: może warto dodać?

![image](https://user-images.githubusercontent.com/116814963/199285898-6893e04b-9e90-4d3e-a57e-8bec68aebf88.png)


