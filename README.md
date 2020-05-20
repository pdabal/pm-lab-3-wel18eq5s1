# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Kordian Kucharek  
Numer albumu: 69102  
Grupa studencka: WELE18Q5S1

# Odpowiedzi do pytań z instrukcji
Zadanie 3.2.2a
Odpowiedź:
Po kliknięciu przycisku raz, program zlicza jakby kliknęło się przycisk 3 albo nawet 4 razy, przy przytrzymaniu przycisku 3 sekundy kliknięcia są zliczane cały czas gdy przycisk jest wciśnięty. Taki wynik jest spowodowany tym, że program rozpoznaje stan wysoki przycisku cały czas, gdy jest on naciśnięty. Nie uwzględnia jaki czas jest naciśnięty, ani nie uwzględnia stanu niskiego przycisku.

Zadanie 3.2.2b
Odpowiedź:
Gdy liczba naciśnięć przekroczy określoną ilość, można dodać funkcję, która będzie kasowała ilość naciśnięć i dodać zmienną, która będzie zliczała ilość osiągniętych określonych ilości naciśnięć(np. gdy będzie 100 naciśnięć to liczba_nacisniec się zeruje, a na dodatkowej zmiennej będą zliczane pełne setki).
