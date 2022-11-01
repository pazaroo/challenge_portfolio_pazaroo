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


### Validations

1. Aplikacja działa prawidłowo, nie pozwalając na wprowadzenie liczba zdobytych goli w liczbie dziesiętnej
![image](https://user-images.githubusercontent.com/116814963/198836764-a0556e58-ce8f-4d76-ac67-7a1cbfab5bee.png)

2. Aplikacja działa prawidłowo, nie pozwalając na wprowadzenie liczby zdobytych goli mniejszych od zera
![image](https://user-images.githubusercontent.com/116814963/198841931-d1f41ad1-8475-47e8-a488-690768330954.png)

3. Aplikacja działa z dobrymi wynikami na poziomie ładowania widoku eydcji gracza
 ![image](https://user-images.githubusercontent.com/116814963/198840860-0d6702f7-5eb8-4a16-bd17-39bc9a610383.png)

### Design

1. Aplikacja po przejściu na widok mobilny i przejsciu do sekcji gracze pokazuje ich w formie listy, a nie kart, jak w przypadku wersji webowej, ale poszczególni gracze zlewają się ze sobą wizualnie ze względu na brak przerwy/grubszej linii lub innego elementu wizualnego
![image](https://user-images.githubusercontent.com/116814963/198839023-40d43581-5642-4b3d-b5e4-0e6fd90f44d8.png)

2. Na widoku edycji raportu meczowego, szerokość strony się zwiększa względem widoku w reszcie aplikacji

Widok w edycji raportu
![image](https://user-images.githubusercontent.com/116814963/198841050-986d7468-db95-44ed-8517-5ad9e61d29ca.png)

Widok np. edycji meczu
![image](https://user-images.githubusercontent.com/116814963/198841102-fb509f37-8c6c-4798-98b3-5b868789f8d7.png)
