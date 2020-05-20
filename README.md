# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Szymon Witkowski
Numer albumu: 72040  
Grupa studencka: WEL18EQ5S1

# Odpowiedzi do pytań z instrukcji
Co się dzieje w momencie jednego kliknięcia przycisku, oraz w momencie trzymania przycisku (np. przez 3 sekundy)?. Dlaczego wynik jest nieco inny od spodziewanego?

W momencie nacisnięcia przycisku odrazu zlicza 3 nacisnięcia przycisku. Jeżeli przytrzymamy przycisk to zlicza cały czas nacisnięcia przycisku. Układ działa gdy na wejściu D2 jest stan wysoki, przy klkinięciu przez pewien czas jest ten stan na tym wejściu, a mikrokontroler widzi że w tym czasie trwania może zostać wcisnięty przycisk kilkokrotnie. Kiedy trzymamy przycisk cały czas, to układ myśli ze klikamy cały czas. Wynik jest inny od spodziewanego, ponieważ w kodzie nie ma opóznienia czasowego i pętla zostaje wykonana kilka razy.


W jaki sposób można rozbudować funkcjonalność programu w przypadku gdy liczba naciśnięć przycisku przekroczy określoną ilość?

Możemy zastąpić unsigned int zmienną unsigned long long co zwiększy nam ilość baitów, a co za tym idzie zakres liczbowy. Można wpisać warunek w void loop() dotyczący liczby nacisnięć.


W jaki sposób można zwiększyć liczbę obsługiwanych poleceń oraz liczbę obsługiwanych parametrów?

Poprzez dodawanie nowych warunków sprawdzających i dopisywanie nowych parametrów ( else if (!strcmp(paramStr, "sprawdzenieLED")) { if (digitalRead(LED_BUILTIN) == HIGH) Serial.println("wlaczony LED") )