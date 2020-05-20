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
3.2.2a) Co się dzieje w momencie jednego kliknięcia przycisku oraz w momencie trzymania przycisku (np. przez 3 sekundy)? Dlaczego wynik jest nieco inny od spodziewanego?
    Przy pojedynczym wciśnięciu przycisku otrzymujemy 4 wiersze, czyli tak jakby przycisk wciśnięty był 4 razy. Przy przytrzymaniu przycisku cały czas otrzymujemy wiersze wciśnięciu przycisku a po jego puszczeniu otrzymujemy jeszcze 3 wiersze wciśnięcia przycisku. Dzieje się tak ponieważ przy wciśnięciu przycisku pętla w kodzie wykonuje się wielokrotnie, ze względu na czas trwania wciśnięcia przycisku a czas trwania pojedynczej operacji mikrokontrolera. 
3.2.2b) W jaki sposób można rozbudować funkcjonalność programu w przypadku gdy liczba naciśnięć przycisku przekroczy określoną ilość?
    Możemy zastąpić unsigned int zmienną unsigned long long co zwiększy nam ilość baitów a co za tym idzie zakres liczbowy. Możemy również dodać zmienną która będzie zliczała ilość resetów, czyli ile razy przekrocziliśmy zakres wartośći dla danego typu zmiennej.
3.2.3 W jaki sposób można zwiększyć liczbę obsługiwanych poleceń oraz liczbę obsługiwanych parametrów? Należy dodać polecenie po wywołaniu którego nastapi informacja czy dioda jest włączona. 
    Należy dodać zmienną (parametr) która zapamięta  stan diody i bedzie go wyświetlać przy wywołaniu. 
    if(digitalRead(LED_BUILTIN, HIGH)){
        Serial.println("Dioda wlaczona");
    }
    else if(digitalRead(LED_BUILTIN)){
        Serial.println("Dioda wylaczona");
    }
    