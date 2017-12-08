Quelle: Mathematik sehen und verstehen: Schlüssel zur Welt
S 25ff
http://www.arndt-bruenner.de/mathe/scripts/primzahlen.htm(8.12.17)
# Potenzieren mit modulo 
Das Potenzieren von moduln spielt in der Crytographie ebenso eine wichtige Rolle. Der Grund dafür ist, dass es sehr schwer ist potenzen von Großen Zahlen herauszufinden.
Um potenzberechnungen zu machen, die mit großen Zahlen ablaufne behilft man sich verschiederner Potenzgesetze. 

Wichtig für die Kryptographie ist die Ordnung k eines Elementes.
Dabei lautet die regel folgendermaßen: 
> Die Ordnung  eines Elementes k entspricht der kleinsten Zahl für a ^k = 1.
> Das heißt, dass es k verschiedene Potenzen von a gibt. 
> Die Ordnung einer Gruppe G entspricht der Anzahl an elementen.
> ord(G) = |G|

An einem Beispiel Verdeutlicht: 
Die Prime Restklasse von 14 Z*14, hat folgende Potenzierungstabelle: 
--> tabelle einfügen
Die Prime Restklasse hat die Grupppenordnung von 6, da des die Anzahl der Elemente sind. 
1.  Die Elemente 3 und 5 haben eine Ordnung von 6, da die Kleinste Zahl die man für k in 3 ^k mod 14 und 5 ^5 mod 14 einsetzen kann 6 ist. 
2. Die Elemente 9 und 11 haben die Ordnung 3, da 9 ^ 3 mod 14 und 11 ^3 mod 14 1 ergibt und dies die kleinstmögliche Potenz ist. 
3. Das Element 13 hat die Ordnung 2, da die kleinste Potenz hierbei 2 ist. 

Wenn man dies schreibt kann man ein bestimmtes Muster erkennen. Die Ordnung 6, 3 und 6 von den Elementen sind alle Teiler der Gruppenordnung 6. Daraus kann man leiten, dass dies der Grund ist, dass die letzte Zeile der Potenztafel immer 1 ergibt.

Hierraus ergibt sich eine zweite wichtige Regel: 
> Es gilt: Das Element mit der Gruppenordnung potenziert ergibt 1. 
> a ^ |G| = 1 
> Die Elementordnung teilt die Gruppenordnung.

# Anzahl der Teilerfremde Elemente für Primzahlen und Produkte von zwei Primzahlen
Mithilfe überlegungen des Mathematikers Leonard Eulers lässt dich leicht feststellen wie viele teilerfremde Elemente ein oder zwei Primzahlen haben. 
Dies ist wichtig zu wissen, wie wir noch im Verlauf feststellen werden. 
> phi(n) bezeichnet die Anzahl der Elemente in Z*n. --> Mathematisch hinschreiben
> Für primzahlen p ...
> Für Primzahlen p und q...

# Eulerscher Satz
Der Eulerscher Satz ist unter anderem ein weitere wichtiger mathematischer Satz den man in der Kryptographie braucht. Er besagt, dass wenn man ein Element a von Zn* mit der Anzahl der Elementen von Zn* potenziert man immer 1 erhält.
> a^phi(n) mod n = 1

# Kleiner Satz von Fermat
Wenn man den Eulereschen Satz fortführt kommt man bei dem kleinen Satz von Fermat an. Dieser besagt, dass:
> bei p prim --> a^p-1 mod p = 1
> dabei ist a kleiner p und größer 0

## Beispiel
Es ist die Menge Z*14 gegeben. 
Die menge der Teilerfremden Primzahlen kann mit den oberen Überlegungen berechnet werden.
1. Primfaktorzerlegung oder falls es kein Produkt zweier Primzahlen ist berechnung von der Anazahl von Primzahlen bis gewisse Zahl:
> 14/2 = 7
> 14 = 2 * 7
2. Falls es produkt zweier Primzahlen war, anzahl teilerfremde Elemente bestimmen: 
> phi(14) = (2-1)*(7-1)
> phi(14) = 6
3. Anwendung des Eulereschen Satzes:
> a^6 = 1 mod 14
> für alle a ist element Z14*

# Potenzieren in Zn*
Wenn man in der Menge Zn* potenzieren möchte geht dies nach dem Bestimmen der gruppenordnung recht einfach. Man rechnet hierbei im Exponenten mit phi(n). Das heißt, dass die vilefachen der Gruppenordnung im expoenent gar nicht zu Wirkung kommen. Man macht also: 
> a elementn Z*n --> a^k+phi(n)+ r = a^r 
  ## Beipiel 
> Z*20 --> bsp bringen 

