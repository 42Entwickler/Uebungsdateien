# Uebungsdateien
Übungsdateien für unterschiedl. Algorithmen und Datenstrukturen

# Infos auf Youtube
Hier ist der Link zum Kanal: [https://www.youtube.com/c/42Entwickler](https://www.youtube.com/c/42Entwickler)

# Graphen-Datensatz
Hier sind die Infos zu diesem Datensatz zu finden: [youtube](https://youtu.be/gSFcqWc7LNQ) bzw. [youtube](https://youtu.be/hHHA3JuSol0)

# Berechnung der Distanzen zwischen zwei Geo-Koordinaten
Voraussetzungen
Alle Winkel in Radiant (nicht Grad!)
Erdradius:
`R = 6371000 Meter`


Schritt 1: Umrechnung von Grad in Radiant
```
lat1 = lat1 * PI / 180
lat2 = lat2 * PI / 180
lng1 = lng1 * PI / 180
lng2 = lng2 * PI / 180
```

Schritt 2: Differenzen
```
dlat = lat2 - lat1
dlng = lng2 - lng1
```

Schritt 3: Haversine-Formel
```
a = sin(dlat/2)^2 + cos(lat1) * cos(lat2) * sin(dlng/2)^2

c = 2 * atan2( sqrt(a), sqrt(1 - a) )

distance = R * c
```

Ergebnis
```
distance = Entfernung in Metern
```
