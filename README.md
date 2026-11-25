# Stundenzettel – Android-Downloads

Persönliche Arbeitszeiterfassung auf Deutsch, ab Android 10. Arbeitszeiten, Pausen, Stundenkonto, Urlaub und Bereitschaft lassen sich offline verwalten. Bereitschaft dient der Planung und erzeugt keine automatische Stundengutschrift.

Version 0.1.9 ergänzt die optionale Synchronisation mit dem [Stundenzettel-Webportal](https://stundenzettel.itzmayztv.chatgpt.site). Mit einem eigenen Konto per E-Mail und Passwort kannst du Arbeitszeiten, Pausen, Bereitschaftseinsätze und geplante Bereitschaften auch im Web bearbeiten. Jede Person sieht ihre eigenen Daten; die Administration kann alle Konten bearbeiten. Ein ChatGPT-Konto ist nicht erforderlich.

## Installieren und aktualisieren

1. Unter [Releases](https://github.com/nikdwo/Stundenzettel-Updates/releases) die gewünschte **Testversion** öffnen und `Stundenzettel-VERSION.apk` herunterladen.
2. Die APK auf dem Android-Gerät öffnen. Falls Android danach fragt, die Installation für die verwendete Browser- oder Datei-App erlauben und die Installation bestätigen.
3. Ein Update über die vorhandene Stundenzettel-App installieren. **Nicht vorher deinstallieren**, sonst werden lokale Daten entfernt. Vor einem Update empfiehlt sich eine lokale JSON-Sicherung unter Einstellungen.

Unter **Einstellungen → Updates** die Schaltflächen **Updates prüfen** und **GitHub öffnen** (bis 0.1.6: „Nach Updates suchen“ und „GitHub-Releases öffnen“). Die Prüfung wird ausschließlich manuell gestartet und berücksichtigt auch veröffentlichte Testversionen. Download und Installation bestätigst du selbst. Arbeitszeit- und Profildaten werden für die Prüfung nicht übertragen; GitHub erhält die üblichen Verbindungsdaten einschließlich IP-Adresse.

Die Datei `SHA256SUMS.txt` enthält die Prüfsumme der APK. Alle hier angebotenen Updates verwenden dieselbe Paketkennung und denselben Signaturschlüssel. Zertifikat SHA-256: `63a0a7a11c91a1cdec2214d88913b890c1c8822c9547ddfb9ec1af5334e62fb1`.

## App und Web verbinden

Im Web **Konto erstellen** wählen und die E-Mail-Adresse über den zugesandten Link bestätigen. In der App unter **Einstellungen → Web-Synchronisation** mit denselben Zugangsdaten anmelden, die Zuordnung der vorhandenen Daten bestätigen und **Verbinden** wählen.

Bei geöffneter App erfolgt der Abgleich automatisch ungefähr alle fünf Sekunden sowie nach lokalen Änderungen. Android kann Hintergrundabgleiche verzögern. Ohne Verbindung bleiben App-Einträge lokal gespeichert. Bei widersprüchlichen Änderungen desselben Eintrags fordert **Konflikte prüfen** eine Auswahl der gültigen Fassung. **Abmelden** erhält die lokalen Daten und ihre Kontozuordnung; eine andere Person kann diesen Bestand nicht mit ihrem Konto übernehmen.

Urlaub, Krankheit, Sollzeiten und persönliche Einstellungen bleiben auf dem Handy. Für einen vollständigen Gerätewechsel deshalb weiterhin eine JSON-Sicherung verwenden. Eine Wiederherstellung kann beim nächsten Abgleich auch Webeinträge ändern oder löschen.

## Grenzen der Testversion

- Die Google-Drive-Anbindung befindet sich nach dem dokumentierten Einrichtungsstand im OAuth-Testbetrieb. Weitere Google-Konten müssen ausdrücklich als Testnutzer freigeschaltet werden; deren Berechtigungen können nach sieben Tagen ablaufen. Lokale Erfassung, Exporte und Dateisicherungen benötigen diese Freischaltung nicht.
- Automatische Feiertagsregeln gelten ab 2020 und benötigen örtliche Korrekturen, wo Feiertage nicht landesweit gelten.
- Version 0.1.6 erfasst tatsächliche Bereitschaftseinsätze per Timer oder Nachtrag. Auswertung und Monatsberichte zeigen sie separat, ohne Anrechnung aufs Stundenkonto.
- Version 0.1.8 zeigt Urlaub (U), Krankheit (K) und geplante Bereitschaften (B) gemeinsam im Kalender. Unter **Einstellungen → Kalenderansicht** lässt sich jede Kategorie einzeln ein- oder ausblenden; die Auswahl bleibt gespeichert.
- Neue Sicherungen verwenden ab 0.1.8 Format 6 und benötigen Version 0.1.8 oder neuer. Formate 1–5 bleiben importierbar; ein Downgrade ist nicht unterstützt.

Dieses Repository enthält ausschließlich öffentliche Downloadinformationen und signierte APKs. Der App-Quellcode wird separat privat verwaltet. Die von GitHub automatisch angebotenen Quellarchive dieses Download-Repositorys enthalten lediglich dessen Dokumentation.
