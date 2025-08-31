# Java Currency Converter

## Projektbeschreibung
Der Java Currency Converter ist eine plattformunabhängige Konsolenanwendung, die Beträge zwischen verschiedenen Währungen umrechnet.  
Das Programm nutzt eine öffentliche API für aktuelle Wechselkurse und speichert diese lokal im Cache, um auch ohne dauerhafte Internetverbindung funktionsfähig zu bleiben.  

Es eignet sich sowohl als Lernprojekt für Java-Einsteiger im Bereich HTTP-Anfragen, JSON-Verarbeitung und BigDecimal-Arithmetik als auch als praktisches Tool im Alltag.

---

## Features
- Umrechnung beliebiger Beträge zwischen über 160 Währungen  
- Live-Wechselkurse über die Open Exchange Rate API (er-api.com)  
- Lokaler Cache für 12 Stunden → schnellere Berechnungen und Offline-Modus  
- Exakte Berechnung mit BigDecimal (kein Rundungsfehler wie bei double)  
- Einfache Bedienung über die Konsole  
- Fallback-Werte, falls weder API noch Cache erreichbar sind  

---

## Technologien
- Programmiersprache: Java 17+  
- Build Tool: Maven  
- Bibliotheken:  
  - Gson (für JSON-Verarbeitung)  
  - Java HttpClient (für API-Requests)  

---

## Nutzung
1. Projekt mit Maven bauen:
   ```bash
   mvn clean package
2. Starten:
    ```bash
    java -jar target/currency-converter-1.0.0-jar-with-dependencies.jar
3. Beispiel Eingabe:
    ```bash
    Betrag (oder 'exit'): 100
    Von Währung (z.B. EUR): EUR
    Nach Währung (z.B. USD): USD

## Lernziele

- Umgang mit HTTP-Requests in Java

- Nutzung von APIs und Parsing von JSON-Daten

- Arbeiten mit Maven als Build Tool

- Fehlerbehandlung und Fallback-Strategien

- Saubere Berechnungen mit BigDecimal
