source: Mathematik sehen vertehen s 29ff.

# Erweiterter Eulidischer Algorithmus 

## Größter gemeinsamer Teiler(ggT)
In der Kryptographie ist das überprüfen von einem Größten gemeinsamen Teiler von Bedeutung. Der größte gemeinsame Teiler(ggT) wird folgendermaßen definiert:
> "Zahlen, die nur die Zahl 1 als gemeinsamen Teiler haben, werden als teilerfremd (relativ prim) bezeichnet."

source:http://www.mathe-lexikon.at/arithmetik/natuerliche-zahlen/teilbarkeit/teilerfremd-relativ-prim.html(10.12.17)  
Für die Kyrptographie wichtig, ist die Frage ob der ggT 1 ist. Denn wenn der ggT von 2 zahlen 1 ist, sind diese Teilerfremd(relativ prim) zueinander. Dies ist für die primen Restklassengruppen in Z*a von bedeutung, wie schon im oberen Teil beschriebe wurde.  
Zusammengefasst gilt folgende Regel:
> 2 Zahlen a,b sind teilerfremd wenn der ggT 1 ist  
> Die zu a teilerfremde Elemente Za fasst man in der Menge Z*a zusammen
> b element von Z*a --> ggT(a,b) = 1

### Beispiel zur bestimmung des ggT
Zur bestimmung des ggT von zwei Zahlen benutzt man einfach die primfaktorzerlegung.
> Gesucht ist der ggT(240, 100)
> Beispiel in Tabelle machen

## Berechnung der Vielfahchen von 2 Teilerfremde Zalen die 1 ergeben durch den erweiterten euklidischen Algorithmus
Wenn der ggT jedoch nicht 1 ist kann man trotzdem mithilfe von 2 Zahlen die 1 darstellen.  
Man hat also: 
> 1 = s * a + t * b

Die gesuchten größen s und t können durch Folgendes Vorgehen berechnet werden: 
1. Berechnen des ggT beider Zahlen
2. Linearkombination erstellen
3. s und t bestimmen

### Beispiel zum erweiterten euklidischen Algorithmus 
> Bsp Tafelanschrieb schreiben 