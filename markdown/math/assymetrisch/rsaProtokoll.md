# RSA Protokoll
Das Diffie Hellmann Protokoll wird in der Kryptographie hauptsächlich zum Schlüsselaustausch genutzt. Das RSA Protokoll kann man im Gegensatz neben dem Schlüsselaustausch zum codieren und Austauschen von Information sowie vom signieren von Nachrichten verwenden.

## Vorgehen
Das RSA Protokoll basiert auf zwei Schritten. Zum einen auf das erstellen der Privaten und Öffentlichen Schlüssel, sowie der verschlüsselung, versendung und entschlüsselung von Nachrichten. Dabei wird eine Nachricht m(Nachricht) mit dem öffentlichen Schlüssel des Empfängers Verschlüsselt. Der empfänger bekommt den Geimtext c und entschlüsselt dieser mit dem privaten Schlüssel d.  
Die Grundlage bilden hier Einwegfunktionen, bei dem man einfach einen Wert berechnen kann aber nur schwer rückrechnen kann.
Die Einwegfunktion ist dabei die Potenzfunktion zum verschlüseln der Nachricht. Bei der Potenzfunktion c = m^ e kann man leich c berechnen, jedoch nur schwer wenn man nur c und e hat. Möglich wird dies nur wenn man den privaten Schlüssel d hat mit dem man die Nachricht c entschlüsseln kann.  

### Schlüsselerzeugungsphase
Die Schlüsselerzeigungsphase gliedert sich in 5 Schritten: 
1. Als erstes wählt man zwei Primzahlen p und q.
2. Die zuvor gewählten Primzahlen werden zu einer Zahl N multipliziert. 
3. Mit dem Satz von Euler berechnet man dann phi(n)
4. Man bestimmt eine Primzahl e, wobei e mit ggT(e, phi) = 1.  
Der Public Key bestimmt sich dabei aus den Zahlen N und e
5. 
--> Überabeiten oder auslassen 


--> Überabeiten, master & vlt Beispiel ?
--> Übern 