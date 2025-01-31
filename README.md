# Confluence Chatbot CLI

## Projektübersicht
Dieser Chatbot ermöglicht die Interaktion mit Confluence direkt über die Kommandozeile (CLI). Er bietet Funktionen zum Suchen, Bearbeiten und Erstellen von Seiten, ohne dass die Confluence-Weboberfläche genutzt werden muss.

Das Projekt richtet sich an Anwender, die grundlegende Automatisierungen für Confluence durchführen möchten oder eine einfache Möglichkeit zur Verwaltung von Inhalten über die API benötigen.

## Funktionen
**Seiten suchen**  
Ermöglicht die Suche nach Confluence-Seiten anhand eines Titels oder Stichworts.

**Seiten bearbeiten**  
Bestehende Seiten können im Titel oder Inhalt geändert werden. Frühere Versionen bleiben erhalten.

**Neue Seiten erstellen**  
Erstellung neuer Seiten in einem vordefinierten Bereich (Space) innerhalb von Confluence.

**Fehlerhandling & Logging**  
Alle API-Anfragen werden protokolliert. Fehlerhafte Anfragen werden automatisch erneut ausgeführt.

**Sichere API-Schlüsselverwaltung**  
Zugangsdaten werden in `config.json` gespeichert und nicht im Code hinterlegt, um die Sicherheit zu gewährleisten.

## Fehlerbehandlung & Sicherheit
- **Logging:** Aktionen werden in `security.log` dokumentiert.
- **Automatische Wiederholung:** Fehlgeschlagene API-Anfragen werden bis zu fünfmal wiederholt.
- **Eingabeprüfung:** Ungültige oder leere Eingaben werden abgefangen und führen zu einer erneuten Abfrage.

## Lizenz
Dieses Projekt steht unter der **MIT-Lizenz**. Weitere Informationen sind in der `LICENSE`-Datei enthalten.

