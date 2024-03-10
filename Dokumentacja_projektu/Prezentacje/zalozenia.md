# Wst�p
G��wnym za�o�eniem projektu jest zaprojektowanie i zbudowanie urz�dzenia umo�liwiaj�cego testowanie przetwornic napi�cia typu DC/DC. Odbywa� si� to b�dzie poprzez dedykowany zasilacz oraz uk�ad sztucznego obci��enia, sterowane przez mikrokontroler. Zakres napi�� wejsciowych, jak i maksymalnych pr�d�w, mocy obci��enia, mo�na b�dzie wybra� poprzez interfejs uzytkownika wyposa�ony w wyswietlacz, przyciski i enkodery inkrementalne. Wyniki wyswietla� mo�na na wbudowanym wyswietlaczu, b�dz przesy�a� poprzez USB do komputera, w formie np. pliku CSV. Maksymalne napi�cie wejsciowe testowanej przetwornicy to 25V, pr�d 4A. Podobnie te�, obi��enie mo�e przyjmowa� napi�cia do 25V i pr�d do 4A, jednak maksymalna wydzielana moc mo�e by� ograniczona do ni�szej wartosci. 

## Najwa�niejsze za�o�enia
* Pomiar wydajnosci przetwornic napi�cia
* Maksymalna moc na wyjsciu przetwornicy co najmniej 50W
* Maksymalna moc na wejsciu przetwornicy - 100W (25 V * 4 A)
* Wyswietlacz z interfejsem do kontroli dzialania urz�dzenia
* Mo�liwos� wys�ania danych poprzez USB na komputer
 
## Opcjonalna funkcjonalnos�
* Pomiar regulacji napi�cia wyjsciowego - jak bardzo zmienia si� napi�cie wyjsciowe w zale�nosci od napi�cia wejsciowego i obci��enia
* Pomiar temperatury przetwornicy - wejscie na np. termopar� albo kilka czujnik�w temperatury.
* Wyswietlanie wynik�w pomiar�w na wbudowanym wyswietlaczu
* Izolacja zasilania oraz sztucznego obci��enia, aby nie ��czy� mas wejscia i wyjscia przetwornicy
 
