# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Korneliusz Duduś
Numer albumu: 71972
Grupa studencka: WELE18Q5S1

# Odpowiedzi do pytań z instrukcji
Odpowiedz na pytanie z zadania 3.2.2 - podczas jednorazowego kliknięci układ nalicza 3 kliknięcia a trzymając przycisk przez 3 sekundy zostaje naliczone 7 kliknięć. Jes to spowodowane szybkością pracy układu i zanim zdężymy odcisnąć przycisk uklad sprawdza już kolejne instrukcje warunkowe if.
3.2.2 B - Gdy liczba naciśnięć przekroczy dopuszczalną ilość można dodać funkcje kasującą ilość naciśnięć oraz zmienną zliczającą naciśnięcia i przy pewnej wartości uruchamiającą funkcję kasowania.
3.2.3 - Należy dodać instrukcje else if obsługujące dodatkowe komendy.
lese if (!strcmp(paramStr, "swieci")) {
      if (digitalRead(LED_BUILTIN == HIGH)){
         Serial.println("swieci");
      } else {
         Serial.println("Nie swieci");
      }
