# Parametry projektu

Nazwa: pm-lab-3  
Autor: Tomasz Składanek (tomasz.skladanek@student.wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Tomasz Składanek  
Numer albumu: 72021
Grupa studencka: WEL18EQ5S1

# Odpowiedzi do pytań z instrukcji

Co się dzieje w momencie jednego kliknięcia przycisku, oraz w momencie trzymania przycisku (np. przez 3 sekundy)?. Dlaczego wynik jest nieco inny od spodziewanego?
W przypadku jednego wciśnięcia zliczany jest jeden impuls, w przypadku przytrzymania przycisku program odświeża się w tym czasie kilkukrotnie. W wyniku tego impuls z przycisku naliczony jest wielokrotnie zamiast jednego długiego.

W jaki sposób można rozbudować funkcjonalność programu w przypadku gdy liczba naciśnięć przycisku przekroczy określoną ilość?
Należy dodać polecenie warunkowe (np. if), które w przypadku przekroczenia ilości naciśnięć przycisku wykona określoną przez nas instrukcję. Może to być np. polecenie ustawiające wartość licznika spowrotem na 0, lub przerywające pętlę liczącą i zamiast tego wyświetlającą komunikat o przekroczeniu dopuszczalnych przyciśnięć.

W jaki sposób można zwiększyć liczbę obsługiwanych poleceń oraz liczbę obsługiwanych parametrów?
Należy dodać więcej poleceń czułych na polecenia wpisywane w konsolę PC oraz przypisać im odpowiednie do wykonania instrukcje.