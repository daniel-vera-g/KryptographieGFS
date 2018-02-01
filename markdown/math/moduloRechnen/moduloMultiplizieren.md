Quelle: Mathematik sehen und verstehen: Schlüssel zur Welt

# Modulo Multiplizieren 
In der Cryptographie ist das rechnen mit Modulo sehr wichtig. Hierbei kommt die 0 vor. Sie kommt vor wenn man mit Zahlen multipliziert die einen gemeinsamen Primfaktor mit der Modulzahl haben. 

Da man in der Cryptographie diese sogenennten Nullteiler vermeiden will nimmt man sie aus dem Moduln Zn raus. Dabei ergeben sich dann die Menge aller Zahlen die mit n keinen gemeinsamen Primfaktor haben. Man bezeichnet diese Menge als Z*n
-->  bearbeiten und formel einfügen. 
Die Menge Z*n nennt man auch prime Restklassengruppe von n.
Sie hat die Eigenschaft, alle Zahlen zu haben die keinen gemeinamen Primfaktor haben. Das heißt diese teilerfremde Zahlen den größten gemeinsamen Teiler(ggT) von 1 haben.
--> Verstehen 

Eine Multiplikationstabelle würde dann folgendermaßen aussehen:
--> tabelle einfügen
Hierbei kommt keine Zahl in einer Spalte doppelt vor. 
Überrall wo hierbei eine 1 steht, kann man davon ausgehen dass sie ein Produkt von 2 Zahlen aus der betreffenden Gruppe ist. 
Folgende regel gilt hier: 
> Wenn 2 Elemente a,b ... --> Regel schreiben !

Inverse sind in der Cryptographie sehr wichtig. Dies wird spätestens dann deutlich wenn man sich die Kryptographie in der Praxis anschaut. 
Dort kann man, wie im späteren verlauf zu sehen, mithilfe der Inverse vershlüsselte Zahlen entschlüsseln. 

Im folgenden ein Beispiel welche die wichtigkeit der Inverse verdeutlichen soll:
* Daniel möchte eine Nachricht an Lukas senden.
1. Daniel wählt eine Nachricht m, ein öffentliches Schlüsselpaar (n, e).  
2. Daniel rechnet m ^ e modulo n und sendet das Ergebniss c and 
3. Lukas rechnen m ^ d modulo n und kann die Nachricht entschlüsseln. D steht hierbei für sein privaten Schlüssel.

Wenn man erkennt, dass der öffentliche Schlüssel e invers zum privaten Schlüssel d ist versteht man auch wie wichtig die inversen in der Cryptographie sind. Mit ihnen kann man die Nachrichten nämlich wieder entschlüsseln.
Eine tiefgründigere Erklärung des Verfahrens wird im praktischen Teil näher erkläutert.

Inverse geben ebenso aufschluss auf die Frage warum die Kryptographie so sicher ist.
Das berechnen von den Inversen ist recht einfach. Vorausgesetzt man kennt in diesem Falle die Nachricht m. Kennt man diese nicht ist es sehr schwer bis unmöglich in großen Restklasssengruppen die Inverse zu berechnen.