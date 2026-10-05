<!-- ELUCENIA technical documentation · sistema-de-bethesda-tireoide · de · no clinical/professional/rights approval -->

# Bethesda-System für Schilddrüsenzytologie

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/sistema-de-bethesda-tireoide)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Befundkategorie

`cat`

- `1` — I · Nicht diagnostisch
- `2` — II · Gutartig
- `3` — III · Atypie unklarer Signifikanz (AUS)
- `4` — IV · Follikuläre Neoplasie
- `5` — V · Malignitätsverdächtig
- `6` — VI · Bösartig

## Fassung der Methode

Bethesda Schilddrüse 2023, 3. Auflage: 6 Kategorien, ROM und nukleäre/sonstige AUS; Dokumentenprüfung auf den Code der gewählten Kategorie beschränkt

## Dokumentierte Formel

Sechs Diagnosekategorien mit mittlerem ROM und Bereich, dritte Ausgabe 2023: ein Name pro Kategorie, AUS in Kernatypie und andere Atypien.

## Grenzen und Population

Die Bethesda-Kategorie muss aus einem zytopathologischen Befund einer Schilddrüsen-Feinnadelaspiration stammen und darf nicht vom Rechner zugewiesen werden. Mittleres Risiko und Bereich sind Schätzungen der Ausgabe, keine individuelle Diagnose. Die Ausgabe 2023 behandelt eigene pädiatrische Risiken und Vorgehensweisen; Erwachsenenwerte dürfen nicht automatisch auf Kinder übertragen werden. Bei dieser Prüfung lieferte der direkte Zugang zum Artikel von 2023 nur den Verlagsabstract; die ROM-Tabelle wurde in einer von Dritten bereitgestellten Reproduktion des Originalartikels mit einem Bild geringer Auflösung gelesen. Die reproduzierte Tabelle 2 nennt für AUS einen Bereich von 13–30 %, während der Text desselben Artikels 20–32 % nennt. Diese Bereiche wurden nicht abschließend gegeneinander beurteilt. Der Test prüft nur den gewählten Kategoriecode; ROM bei Erwachsenen, pädiatrischer ROM und das Vorgehen wurden in dieser Prüfung nicht validiert.

## Referenzen

- [Ali SZ et al. The 2023 Bethesda System for Reporting Thyroid Cytopathology. Thyroid, 2023.](https://doi.org/10.1089/thy.2023.0141)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
