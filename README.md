# Python w pigułce


<font size="14"><b>Moje notatki z Pythona</b></font>
<img src="https://github.com/szewa5/moje-projekt/blob/gh-pages/images/waz.png?raw=true" alt="Tu podaj tekst alternatywny" />
<b>1. Podstawowe komendy</b>


include <stdio.h>
#include <math.h>

double Heron (double a);
                        {
doble x=1, eps=1e-15;
    do
    {
        x=0.5*(x+(a/x));
    }
    while (fabs (x-a/x)>eps*x);
    return x;
}
int main(){
    duble a;
    duble x=1;
    doble z;
    pritf("Podaj liczbę: ");
    scanf("%1f", &a);
        for (z=1e-5; z<=1e15; z=z*10)
        {
            printf ("\nHeron(%1f)=%.15lf\n", z, Heron(a));
            printf ("\nsqrt(%1f)=%.15lf\t", z, sqrt(a));
            printf ("\n\nblad wzgledny=%.15le", (Heron(a)
            -sqrt(a)) / sqrt(a));
            getchar ();
            getchar ();
            return 0;
        }
}
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

for zmienna in range(limit):
    instrukcja
np.:
silnia = 1
for j in range(10):
    silnia = silnia * (j + 1)
print(silnia)

while (warunek):
    instrukcja

funkcje:
np:
def a(n):
    kod funkcji z odstępem
a(10)                         wywołanie funkcji

sum(tablica)               zsumowanie wartości komórek tablicy
max(tablica)               zwraca największą wartość w tablicy
min(tablica)                zwraca najmniejszą wartość w tablicy
len(tablica)                 zwraca długość tablicy


import numpy as np

np.sin(liczba)            sinus
np.cos(liczba)           cosinus

np.prod(tablica)           przemnożenie wartości komórek tablicy
np.mean(tablica)         średnia arytmetyczna z zawartości tablicy
np.pi                         liczba pi
np.sqrt()                     pierwiastek z liczby
np.exp()                     wartość eksponencjalna z liczby
np.sort(tablica)           sortowanie tablicy
np.arange(wartość pocz., wartość końc., krok)    tworzy nową tablicę
np.linspace(wartość pocz., wartość końc., liczba punktów)      tworzy nową tablicę
np.transpose(A)          transpozycja macierzy
np.polyval(w1, a)         zwraca wartość wielomianu w1 w punkcie a



import matplotlib.pyplot as plt

plt.plot(oś x, oś y, sposób wyświetlania)          tworzenie wykresu
plt.show()                                pokazanie wykresu na ekranie
mogą być sposoby wyświetlania (można łączyć je ze sobą np. 'o-r' :
'r'        kolor (tutaj czerwony)
'-'        linia ciągła
'--'       linia przerywana
'x'       krzyżyki
'o'       punkty
przykład:
plt.plot(xA,yB,'o-r',yB,xA,'x-y')

plt.xlabel('opis')              opis danej osi, tutaj oś x
plt.legend                      wyświetlenie legendy
plt.grid(True)                  wyświetlenie siatki


import numpy. random as npr

npr.rand(liczba)     liczba losowa rzeczywista od zera do liczba. Dodanie kolejnej stworzy macierz
npr.randint(liczba, size(inna liczba))          liczba losowa całkowita. Dodanie liczby stworzy macierz

import numpy.linalg as npl

npl.solve(A,b)      rozwiązanie układu równań funkcji np. macierzy A i wektora b


from scipy.optimize import fsolve

fsolve(f2, 0.6)              zwraca wartość przybliżonego miejsca zerowego funkcji f2 w pobliżu x = 0.6, czyli pierwiastek funkcji
