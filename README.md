# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Mateusz Klekota
Numer albumu: 69094  
Grupa studencka: WELE18Q5S1

# Odpowiedzi do pytań z instrukcji
...
3.2.2 Co się dzieje w momencie jednego kliknięcia przycisku oraz w momencie trzymania przycisku (np. przez 3 sekundy)? Dlaczego wynik jest nieco inny od spodziewanego?
    Przy pojedynczym wciśnięciu przycisku otrzymujemy 4 wiersze, czyli tak jakby przycisk wciśnięty był 4 razy. Przy przytrzymaniu przycisku cały czas otrzymujemy wiersze wciśnięciu przycisku a po jego puszczeniu otrzymujemy jeszcze 3 wiersze wciśnięcia przycisku. Dzieje się tak ponieważ przy wciśnięciu przycisku pętla w kodzie wykonuje się wielokrotnie, ze względu na czas trwania wciśnięcia przycisku a czas trwania pojedynczej operacji mikrokontrolera. 