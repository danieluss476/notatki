# Python w pigułce


# Moje notatki z pythona
<img src="https://github.com/szewa5/moje-projekt/blob/gh-pages/images/waz.png?raw=true" alt="Tu podaj tekst alternatywny" />

<b>1. Podstawowe komendy:</b>

``` 
a =                       deklaracja zmiennej
print(a)                  drukowanie w konsoli
string1 = 'witaj'       deklaracja napisu
string2 = 'świecie'
print(string1 + ' ' + string2)       drukowanie napisu
#                           komentarz
help(funkcja)          tekst pomocy funkcji
może być:
print('tekst') lub print("tekst")
/                           dzielenie bez reszty. By dzielić z resztą, jedna ze zmiennych musi być zmiennoprzecinkowa
%                          reszta z dzielenia
\                            kontynuacja linii
*                            mnożenie
**                           potęgowanie
s = '3 9 81'
print(s.split())          podzielenie napisu domyślnie spacją. Otrzyma się tablicę wyrazów

tablica.append(liczba)         dopisanie liczby na końcu tablicy (doda nową komórkę)
tablica.insert(pozycja, liczba)    wstawienie liczby w danej pozycji tablicy
len(tablica)                   długość tablicy (liczba komórek)
tablica[pozycja pocz : pozycja końc] = [liczba1, liczba2,... liczban]       zmiana wartości komórek w tablicy w danym zakresie pozycji
tablica[komórka]          wywołanie komórki tablicy
tablica[ ]                   utworzenie nowej pustej tablicy bez zakresu rozmiaru
tablica1 = tablica2[ : ]    skopiowanie tablicy
tablica.reverse()           zamiana kolejności komórek w tablicy

instrukcja warunkowa:
if (warunek):              <= pamiętać o dwukropku!
    instrukcja1            <= wcięcia decydują czy coś jest w instrukcji warunkowej
    instrukcja2
elif (warunek2):
    instrukcja
else:
    instrukcja
```
