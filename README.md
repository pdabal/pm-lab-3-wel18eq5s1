# Parametry projektu

Nazwa: pm-lab-3  
Autor: Paweł Dąbal (pawel.dabal@wat.edu.pl)  
Opis: Projekt bazowy repozytorium na trzecie spotkanie laboratoryjne z przedmiotu _Programowanie mikrokontrolerów_.  
Wersja: v1.0  
Data: 20.05.2020 r.

# Informacje o studencie

Imię i nazwisko studenta: Michał Kłosiewicz 
Numer albumu: 69095
Grupa studencka: WEL18Q5S1

# Odpowiedzi do pytań z instrukcji
Odpowiedź do zadania 3.2.2.a:
W momencie wciśnięcia przycisku na porcie szeregowym otrzymujemy więcej niż jedną informację. Wynika to z tego, że pętla odpowiedzilna za zliczanie wykonuje się więcej ni jeden raz, ponieważ nie posiada ograniczenia funkcją delay(). Gdy przycisk przytrzymamy 3 sekundy otrzymujemy znacznie więcej informacji o wciśnięciu przycisku.
  

Odpowiedź do zadania 3.2.2.b:
Możemy zwiększyć ilość baitów przez zastosowanie zmiennej long long.


Odpowiedź do zadania 3.2.3:
Należy dodać kolejną instrukcję if.
if(digitalRead(LED_BUILTIN, HIGH)){
  Serial.println("Dioda jet wlaczona");
} else
{
  Serial.println("Dioda jest wylaczona");
}