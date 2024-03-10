# Wstêp
G³ównym za³o¿eniem projektu jest zaprojektowanie i zbudowanie urz¹dzenia umo¿liwiaj¹cego testowanie przetwornic napiêcia typu DC/DC. Odbywaæ siê to bêdzie poprzez dedykowany zasilacz oraz uk³ad sztucznego obci¹¿enia, sterowane przez mikrokontroler. Zakres napiêæ wejsciowych, jak i maksymalnych pr¹dów, mocy obci¹¿enia, mo¿na bêdzie wybraæ poprzez interfejs uzytkownika wyposa¿ony w wyswietlacz, przyciski i enkodery inkrementalne. Wyniki wyswietlaæ mo¿na na wbudowanym wyswietlaczu, b¹dz przesy³aæ poprzez USB do komputera, w formie np. pliku CSV. Maksymalne napiêcie wejsciowe testowanej przetwornicy to 25V, pr¹d 4A. Podobnie te¿, obi¹¿enie mo¿e przyjmowaæ napiêcia do 25V i pr¹d do 4A, jednak maksymalna wydzielana moc mo¿e byæ ograniczona do ni¿szej wartosci. 

## Najwa¿niejsze za³o¿enia
* Pomiar wydajnosci przetwornic napiêcia
* Maksymalna moc na wyjsciu przetwornicy co najmniej 50W
* Maksymalna moc na wejsciu przetwornicy - 100W (25 V * 4 A)
* Wyswietlacz z interfejsem do kontroli dzialania urz¹dzenia
* Mo¿liwosæ wys³ania danych poprzez USB na komputer
 
## Opcjonalna funkcjonalnosæ
* Pomiar regulacji napiêcia wyjsciowego - jak bardzo zmienia siê napiêcie wyjsciowe w zale¿nosci od napiêcia wejsciowego i obci¹¿enia
* Pomiar temperatury przetwornicy - wejscie na np. termoparê albo kilka czujników temperatury.
* Wyswietlanie wyników pomiarów na wbudowanym wyswietlaczu
* Izolacja zasilania oraz sztucznego obci¹¿enia, aby nie ³¹czyæ mas wejscia i wyjscia przetwornicy
 
