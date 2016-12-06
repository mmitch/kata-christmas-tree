# Weihnachtsbaum-Kata

Diese Kata ist eine recht simple Kata, die sich hauptsächlich mit
String- und Textbearbeitung beschäftigt.  Sie ist der _Diamant-Kata_
ähnlich.

## Ziel der Kata

Erstelle die Textdarstellung eines Weihnachtsbaumes für eine bestimmte
Baumhöhe.

Ein ordentlicher Weihnachtsbaum besteht aus diesen drei Teilen:

* einem Stern auf der Spitze
* dem grünen Teil dazwischen _(wenn jemand ein schönes Wort dafür hat:
  lasst es mich wissen)_
* dem Stamm

Der Weihnachtsbaum soll für eine Festbreitenschriftart berechnet
werden, in der jeder Buchstabe gleich breit ist, so wie in diesem
String:  `"iiimmm"`.

## Baumhöhe

Die Baumhöhe soll nur einstellig sein, die zu berücksichtigenden Höhen
liegen also im Bereich von `0` bis `9`.

## Stern auf der Spitze

Die Spitze des Weihnachtsbaumes soll mit einem Stern geschmückt sein,
der durch das Zeichen `*` dargestellt wird.  Der Stern soll sich in
der gleiche Spalte wie der Stamm befinden.

## Der grüne Teil in der Mitte

Die Äste und Nadel des Weihnachtsbaumes sollen durch mehrere Zeilen
repräsentiert werden:

* Die erste Zeile soll nur die Zahl `1` enthalten.
* Die zweite Zeile soll die Zahl `2` zwei Mal enthalten, getrennt
  durch ein Leerzeichen.
* Die dritte Zeile soll die Zahl `3` drei Mal enthalten, wieder
  jeweils durch ein Leerzeichen getrennt.
* Und so weiter.

Die `1` in der ersten Zeile soll in der gleichen Spalte wie der Stern
und der Stamm dargestellt werden.  Die weiteren Zeilen sollen davon
ausgehend gleichmäßig nach links und rechts wachsen.

Die Höhe dieses Teiles des Baumes hängt von der gewünschten Baumhöhe
ab:

* Eine Baumhöhe von `0` lässt diesen Teil komplett entfallen.
* Eine Baumhöhe von `1` erzeugt in diesem Teil nur eine Zeile mit der
  Zahl `1`.
* Eine Baumhöhe von `2` erzeugt in diesem Teil zwei Zeilen, eine mit
  einer `1` und eine mit zwei `2`en.

Ein Bild sagt mehr als tausend Worte, daher bitte einmal unten in die
Beispiele gucken.

## Stamm

Der Stamm ist das nackige Stück Holz, das unten aus dem grünen Teil
rausguckt.  Er soll durch das Zeichen `#` dargestellt werden.  Der
Stamm soll sich in der gleichen Spalte wie der Stern auf der Spitze
befinden.

Der Stamm ist immer genau eine Zeile hoch, selbst in den größten
Bäumen.

## Beispiele

Höhe 0:
```
*
#
```

Höhe 1:
```
*
1
#
```

Höhe 2:
```
 * 
 1 
2 2
 # 
```

Höhe 3:
```
  *  
  1  
 2 2 
3 3 3
  #  
```

Höhe 4:
```
   *   
   1   
  2 2  
 3 3 3
4 4 4 4
   #   
```

## Zusatzaufgaben

* Baue Bäume für zweistellige Höhen.
  * Bevor Du anfängst: Welche Schwierigkeiten erwartest Du?
  * Welche Probleme siehst Du, wenn Du einen Baum mit der Höhe `10`
    erstellst?
  * Wie kannst Du diese Probleme lösen?
  * Wie kommt Dein bestehendes Design mit diesen neuen Anforderungen
    zurecht?

* Baue Bäume, die um eine oder mehrere Größenordnungen höher
  sind. (Versuche nur, sie zu generieren; es wird schwierig werden,
  sie ordentlich anzuzeigen oder zu testen, ob sie korrekt sind.)
  * Bevor Du anfängst: Welche Schwierigkeiten erwartest Du?
  * Welche Probleme siehst Du, wenn Du einen Baum mit der Höhe `100`,
    `1000` oder `10000` erstellst?
  * Wie kannst Du diese Probleme lösen?
  * Wie kommt Dein bestehendes Design mit diesen neuen Anforderungen
    zurecht?
