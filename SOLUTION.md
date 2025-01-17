# **SWO3-Übungen - WS2023/24 - Übungszettel 2 - Ausarbeitung**

## **Beispiel 1**

#### **a)**

So wie die Schnittstelle definiert ist, sieht es so als würde das Polynom "4 + 3*x - 2*x^2 + x^3" so p = {4, 3, -2, 1} im Array p abgespeichert sein. Wobei die Variable m die höchste Potenz angibt. Zum Ausgeben, würde ich eine eigene Funktion schreiben, die in einer For-Schleife über alle Elemente des Arrays iteriert und diese ausgibt. Dabei muss unterschieden werden zwischen + und - und dem Sonderfall x^0 (gar nicht anzeigen) und wenn ein Koeffizient 1 ist soll er auch nicht angezeigt werden. Annahme: Koeffizienten sollen in der Ausgabe als Integer dargestellt werden wie in der Angabe.

#### **b)**

Um den Wert des Polynoms an einer Stelle zu berechnen kann man einfach den Wert eines jeden Terms berechnen und dann die Summe bilden. Wobei man jeweils für x einsetzt und die Potenz berücksichtigt.

#### **c)**

Um zwei Polynome zu addieren, muss man nur deren Koeffizienten paarweise addieren. Dies kann man mit einer For-Schleife machen. Um die Grenze der Schleife zu ermitteln, nimmt man einfach das größere der zwei Eingangsarrays.

#### **d)**

Um zwei Polynome zu multiplizieren, muss jeder Koeffizient des einen Polynoms mit jeweils allen Koeffizienten des anderen Polynoms multipliziert werden. Diese Aufgabenstellung klingt nach zwei For-Schleifen. Die Grenzen der Schleifen sind jeweils die Potenz des Eingangarrays.

#### **e)**

Hier muss man zwei Polynome mit dem Prinzip Teile- und Herrsche multiplizieren. Dabei wird angenommen, dass die beiden Polynome den gleichen Grad haben und die Länge eine Zweierpotenz ist. Die Polynome werden in vier gleich große Hälften aufgeteilt, und mithilfe von Hilfsvariablen wird das Produkt berechnet. Die Funktion muss sich rekursiv so lange selbst aufrufen, bis das Teilproblem gleich genug ist um es zu lösen und nachher wird wieder kombiniert.

### **Lösungsidee**

### **Testfälle**

#### **a)**

Tests zur Ausgabe, negative Potenz ungültig. Annahme Anzeige soll auf ganze Zahlen gerundet werden wie in der Angabe.

![](doc/poly1.png)

![](doc/poly2.png)

#### **b)**

Tests zur Berechnung des Polynoms

![](doc/poly3.png)

![](doc/poly4.png)



#### **c)**

Test zum Addieren von Polynomen und Angabe des Grades

![](doc/poly5.png)

![](doc/poly6.png)

#### **d)**

Test zum Multiplizieren von Polynomen und Angabe des Grades

![](doc/poly7.png)

![](doc/poly8.png)

#### **e)**

Test zum Multiplizieren von Polynomen und Angabe des Grades

![](doc/poly9.png)

![](doc/poly10.png)