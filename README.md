# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Damian Duchnowski  
Numer albumu: 69072
Grupa studencka: WELE18Q5S1

# Odpowiedzi do pytań z instrukcji
...
Co się dzieje w momencie jednego kliknięcia przycisku oraz w momencie trzymania przycisku (np. prze 3 sekundy)? Dlaczego wynik jest nieco inny od spodziewanego?
Program działa w taki sposób, iż gdy naciśniemy raz przycisk, wtedy program wyświetli komunikat nieco mylący- według programu przycisk został naciśnięty 4 razy. Jeśli przetrzymamy ten sam przycik dłużej (właśnie np przez 3 sekundy) to liczba naciśnięć na konsoli będzie 3krotnie większa (w tym przypadku 12).

W jaki sposób można rozbudować funkcjonalność programu w przypadku gdy liczba naciśnięć przycisku przekroczy określoną ilość?
Można dodać  granicę licznika "liczba_naciśnięć", która będzie działać w taki sposób, iż po przekroczeniu określonej wartości uruchomi diodę LED, która będzie sygnalizowała na płytce przerwanie liczenia.