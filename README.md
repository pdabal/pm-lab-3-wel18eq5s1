# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Imię Nazwisko  
Numer albumu: 12345  
Grupa studencka: WELE18Q5S1

# Odpowiedzi do pytań z instrukcji
odp do zadania 3.2.2:
    Po wciśnięciu przycisku, w monitorze portu szeregowego, otrzymujemy więcej niż jedna informację dotyczącą wciśnięcia przycisku
    (po wciśnięciu przycisku przes 3 sekundy otrzymujemy ich całą masę). Spowodowane jest to tym, iż po wciśnięciu przycisku, pętla odpowiedialna za zliczanie i wysłanie informacji wykonuje się wiecej niż jeden raz ponieważ nie posiada ograniczenia np. w postaci funkci delay() (wykoanie pętli trwa znacznie krócej niż czas wciśnięcia przycisku).

odp do zadania 3.2.2b:
    By zwiększć ilość moliwych zliczeń licznika umieszczonego w pętli należy zmienić zmienną odpowiedzialną za przechowywanie ilości zliczeń na większą np. na "unsigned long long", która umożliwia przechowowyanie większych liczb. 

odp do zadania 3.2.3:
    należy dodać koleny warunek else if posiadający wymagane przez nas polecenie.