# Inversenbestimmung modulo n
Da die berechnung von Inversen modulo n sehr schwierig ist, stellt die Inversenbestimmung eine sehr wichtige Säule in der modernen Kryptographie dar. Um Inverse modulo n zu betimmen gibt es verschiedene möglichkeiten.

## 1. Multiplikationstafel
Man schaut sich die Multiplikationstafel an und schaut bei welchen Zeilen und Spalten sich eine 1 befindet. Diese sind Invers zueinander.  
## 2. Potenztafel
Man schaut sich die Potenztafel an und schaut welche Zahl sich über der ersten 1 befindet. Diese zahl ist invers zu der ausgesichten Zahl a.
> Bsp Bringen
## 3. Kreisvisualisierung 
Man kann sich die Modulo rechnung wie ein Kreis Vorstellen und dort wo ...
> Bsp oder falsch nocht verstehen auslassen 
## Problem bei großen Moduln
Die vorhergehenden Methdoden sind in der Theorie wirksam, jedoch für große Moduln unpraktisch. Hierbei nutzt man eine weitere Methode, die weitaus effizienter ist. Diese Methode nennt sich erweiterter euklidische Algorithmus.  
Bei diesem nimmt man eine Zahl e element von Z*k und kann im folgenden den Inversen bestimmen und ob sich e überhaupt in Z *k befindet.
Dabei macht man folgende Rechnung: e * d = 1 mod k.  
Da dieser Algorithmus in der Kryptographie relativ wichtig ist, wird er im folgenden näher beschrieben.