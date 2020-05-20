# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Aleksy Pazura
Numer albumu: 72006
Grupa studencka: WELE18Q5S1

# Odpowiedzi do pytań z instrukcji
Pytanie 1. 
Co się dzieje w momencie jednego kliknięcia przycisku, oraz w momencie trzymania przycisku (np. przez 3 sekundy)? Dlaczego wynik jest nieco inny od spodziewanego.

Gdy kliniemy przycisk w odpowiedzie otrzymamy informację, że kliknęliśmy przycisk np 4 razy, gdy przytrzymamy przycisk przez 3 sekundy zaczną naliczać się następne kliknięcia mimo, że trzymamy przycisk. Wynik jest inny od spodziewanego ponieważ program wykonywany jest w pętli i zanim zdązymy puścić przycisk program zdąży wykonać się już kilka razy.

Pytanie 2.
W jaki sposób można rozbudować funkcjonalność programu w przypadku gdy liczba naciśnięć przyisku przekroczy określoną liczbę?

Można dodać zmienną która będzie zerowała pierwszą zmienną, jeśli ta przekroczy określoną liczbę.

Pytanie 3.
W jaki sposób można zwiększyć liczbę obsługiwanych poleceń oraz liczbe obsługiwanych parametrów?

Poprzez dodanie ich do kodu, opisanie ich działania w danym przypadku.