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
