# Dairy 20.03.2020

(ausnahmsweise auf Deutsch weil Zitat aus LinkedIn Learning Kurs)
## Wie entscheidet der Browser, welche CSS-Regel er anwendet?
* Zuerst sammelt der Browser alle passenden Anweisungen.
* Wenn er keine findet, um etwas zu gestalten, dann prüft er, ob Vererbung stattfindet. Und wenn er nichts findet über die Vererbung, also entweder weil die Eigenschaft nicht vererbt wird oder weil in diesem Dokument nichts definiert wurde, dann wendet er den Standardwert an.
* Wenn er genau eine Anweisung findet, dann nimmer er den Wert und fertig.
* Normalfall ist jedoch, dass der Browser mehrere Anweisungen findet, um ein und dieselbe Stelle zu gestalten und dann durchläuft er die Kaskade.
* Die Kaskade besteht aus drei Schritten:
  * Erstens guckt er, ob eine Anweisung ```!important``` hat.
  * Wenn das nicht der Fall ist, dann schaut er nach der Spezifität.
  * Und wenn auch da sich nichts ergibt, dann schaut er nach der Reihenfolge (die Anweisung ganz unten wird verwendet)