Source: http://ddi.uni-wuppertal.de/material/spioncamp/dl/austausch-diffie-hellman-station2.pdf(10.12.17)
http://ddi.cs.uni-potsdam.de/Lehre/e-commerce/elBez2-5/page07.html(01.12.17)

# Diffie-Hellman Algorithmus
Der Diffie-Hellman Algorithmus, ist ein Algorithmus welches als einer der ersten dass erstellen eines gemeinsamen Schlüssels durch einer unsichere Verbindung ermöglichte. Dabei beutzen beide Verbindungspartner den gleichen Schlüssel.
## Vorgehen
Zwei Personen(In diesem Beispiel Alice und Bob) vereinbaren eine Primzahl p und eine natürliche Zahl g. Dabei muss g < p gelten.
### Verschlüsselung
* Alice:
1. Alice wählt eine Zahl a, wobei a < p ist.
2. Alice rechnet g^a mod p = A. 
3. Alice sendet A and Bob.  

* Bob:
1. Bob wählt Zahl b, wobei b < p ist.
2. Bob rechnet g^b mod p = B.
3. Bob sendet B and Alice.
### Entschlüsselung
* Alice
1. Alice rechnet B^a mod p = K, wobei K der gemeinsame geheime Schlüssel ist.

* Bob
1. Bob rechnet A^b mod p = K, wobei K der gemeinsame geheime Schlüssel ist.

#### Beispiel des Dieffie-Hellman Algorithmus
> Bsp rechene

## Angriff auf den Diffie-Hellman  Algorithmus
Die Schwäche des Diffie-Hellman algortithmus liegt im privaten Schlüssel, der kleiner als die Primzahl sein muss. Damit eine Person den Geheimen Schlüssel berechen könnte, bräuchte er entweder die geheime Zahl von Alice oder Bob. Da diese Zahl kleiner als die Primzahö ist und die Person die Primzahl kennt muss er nur noch so lange ausprobieren bis er zufällig auf die Zahl stößt.  
Er könnte ebenso auf andere kryptographische Verfahren zurückgreifen die dies ermöglichen. Da diese weiteren Verfahren jedoch den den Rahmen sprengen würden und nicht mit dem eigentlichen Grundthema dieser GFS vereinbar sind, werde ich auf die weitere Eerläuterungen dieser Verfahren verzichten.
> verfahren falls zeit und lust noch weiter erklären

## Anwendung des Diffie-Hellman Algorithmus
Der Diffie-Hellman Algorithmus ist die Grundlage für für weitere Verschlüsselungstechniken. Die Anwendung des Diffie-Hellman Algorithmus in Kombination mit anderen Austauchprotokollen sieht folgendermaßen aus: 
1. Man erzeugt mithilfe des Diffe-Hellman algorithmus wie oben gezeigt ein geheimen Schlüssel.
2. Man wählt ein Symmetrisches Verschlüsselungsverfahren um Nachricht zu verschlüsseln.
Solche Verfahren, die symmetrische und asymetrische Verfahren kombinieren werden auch hybride Verschlüsselung gennant.  
Der Vorteil der hybriden Verschlüsselung gegenüber vollkommen assymetrische Verfahren liegt im Rechenaufwand. Dieser ist bei der hybriden Verschlüsselungen geringer.