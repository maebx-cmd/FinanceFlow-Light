# FinanceFlow Light

**Schulden erfassen am Smartphone – für die Schuldenberatung.**

👉 **Zur App: https://maebx-cmd.github.io/FinanceFlow-Light/**

FinanceFlow Light ist die Smartphone-Version von FinanceFlow für Schuldnerinnen und Schuldner, die keinen Computer
oder Laptop haben. Die ganze App ist eine einzige HTML-Datei (`index.html`, ca. 50 KB) ohne externe Bibliotheken,
Schriften oder Server.

## Was die App kann

- **Gläubiger anlegen** – Name, Adresse, Telefon, E-Mail, IBAN (mit Prüfung), Notizen
- **Schulden erfassen** – Gläubiger, Bezeichnung, offener Betrag, Rate und Fälligkeitstag, Zinssatz, Privatkonkurs ja/nein
- **Neuer Betrag** aus einem Brief oder nach einer Zahlung – wird nachvollziehbar als Korrektur mit Art, Datum und
  Beschreibung gespeichert
- **Startseite** mit offener Summe, Raten pro Monat und „Erste Schritte“
- **Einführung in einfacher Sprache**
- **Beträge verbergen** und **Sperren**
- **Datei für die Schuldenberatung** erstellen und über das Teilen-Menü (E-Mail, Messenger …) senden;
  **Datei der Beratung** öffnen

## Datenschutz

- Die Seite wird nur geladen – **es werden keine Daten gesendet**. Alles bleibt im Browser des Handys.
- Der Datenstand ist im Browser **verschlüsselt** (Passwort des Benutzers, PBKDF2-HMAC-SHA256 mit 600.000 Iterationen,
  AES-256-GCM).
- Die Datei für die Beratung (`*.ffsync`) ist mit einem eigenen Passwort (mindestens 12 Zeichen) verschlüsselt. Das
  Passwort wird getrennt von der Datei weitergegeben, am besten telefonisch.
- Werden die Browserdaten gelöscht oder geht das Handy verloren, ist der Stand am Handy weg. Die zuletzt erstellte
  Datei ist deshalb zugleich die Sicherung – die App erinnert daran.

## So wird sie verwendet

1. Link öffnen (Safari, Chrome, Samsung Internet …) und im Browser-Menü **„Zum Home-Bildschirm“** wählen.
2. Name und Passwort festlegen, die Einführung durchblättern.
3. Zuerst alle **Gläubiger** anlegen, dann die **Schulden** erfassen.
4. Unter **„Datei“** die Datei erstellen und der Schuldenberatung schicken.

Android kann die Datei `index.html` auch direkt öffnen (speichern, mit Chrome öffnen). Am iPhone bitte den Link verwenden.

## Zusammenspiel mit FinanceFlow Schuldenberatung

Die Datei hat dasselbe Format wie FinanceFlow für Windows, Android und iPhone. Die Schuldenberatung spielt sie in
[FinanceFlow Schuldenberatung](https://github.com/maebx-cmd/FinanceFlow-Schuldenberatung) unter
*Mandanten → Datei des Schuldners einspielen* ein und kann einen überarbeiteten Stand als Datei zurückgeben.
Daten, die die App selbst nicht bearbeitet (Haushaltsrechnung, Zahlungspläne, Szenarien, Postbuch …), bleiben dabei
unverändert erhalten.

## Aktualisieren

`index.html` ersetzen und pushen – GitHub Pages veröffentlicht die neue Fassung automatisch.
