# Primzahltest
Wie man aus den bisherigen Schlüsseln sehen kann spielen Primzahlen eine sehr große Rolle in der Kryptographie.  
Die Definition einer Primzahl ist:
>"Eine natürliche Zahl, die nur durch sich selbst und 1 (ohne Rest) teilbar ist"

Source: http://www.arndt-bruenner.de/mathe/scripts/primzahlen.htm(9.12.17)  

Um eine Zahl auf Primzahleigenschaften zu testen muss man also schauen ob sie nur durch sich selbst und 1 Teilbar ist. Für kleine Zahlen ist dies nicht sehr aufwendig.  
In der Kryptographie rechnet man jedoch mit Zahlen die an bis zu den 300 Stelen haben. In diesem Fall, ist das obere Verfahren sehr uneffizient und man muss auf ein weiteres Verfahren zurückgreifen. 

## Primzahltest mithilfe des kleinen Satzes von Fermat
Wenn man für eine Zahl m wissen will ob sie eine Primzahl ist geht man nach dem folgenden Schema vor:

1. Man nimmt irgendeine Zhal a mit 1 < a < m
2. Man rechnet a^m-1 = z mod m
3. * Wenn z > 1 ==> m keine Primzahl aufgrund des kleinen Satzes von Fermat. Der besagt ja dass, a^p-1 = 1 mod p. Wobei p eine Primzahl ist.
    * Wenn z = 1 ==> Probiert man andere Zahlen zur Sicherheit für a aus oder setzt andere aufwendigare Primzahltests ein. Wenn diese nicht scheitern, ist die Zahl eine Primzahl.

### Beispiel eines Primzahlttests mit dem kleinen Satz von Fermat

1. Gegeben ist die Zahl 731
2. Man wählt die Zahl 2 für a aus. 
3. 2^731-1 = 4 mod 731 ==> Keine Primzahl

Source: Mathematik Sehen und Verstehen S 29