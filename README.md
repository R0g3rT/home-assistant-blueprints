# Home Assistant Blueprints

Dieses Repository enthält eine Sammlung von **Home-Assistant-Blueprints** zur einfachen und wiederverwendbaren Erstellung von Automationen.

Die Blueprints sind praxisorientiert aufgebaut, modular konfigurierbar und können **direkt über eine URL** in Home Assistant importiert werden.

---

## 📦 Inhalt

Dieses Repository umfasst mehrere unabhängige Blueprints, unter anderem für:

- Geräte-Status-Erkennung (z. B. „Gerät fertig“ über Leistungsaufnahme)
- Benachrichtigungen und Sprachausgaben (TTS)
- Sensor- und Zustands-basierte Automationen
- Wiederverwendbare Standard-Automationslogik

Jeder Blueprint ist eigenständig nutzbar und kann mehrfach verwendet werden.

---

## 🚀 Installation (empfohlen: URL-Import)

Home Assistant unterstützt den direkten Import von Blueprints über eine URL.

### Blueprint über URL importieren

1. **Home Assistant öffnen**
2. **Einstellungen → Automationen & Szenen → Blueprints**
3. Unten rechts auf **„Blueprint importieren“** klicken
4. Die **Raw-URL** des gewünschten Blueprints einfügen  
   Beispiel:
    https://raw.githubusercontent.com/<USER>/<REPO>/main/<BlueprintName>.yaml
5. **Vorschau** prüfen und **Importieren**

Der Blueprint steht danach sofort zur Verfügung.

---

## 🗂️ Manuelle Installation (Alternative)

Falls kein URL-Import gewünscht ist:

1. Blueprint-Datei (`.yaml`) herunterladen
2. In folgendes Verzeichnis kopieren:
   config/blueprints/automation/<dein_ordner>/
3. Home Assistant neu starten oder Blueprints neu laden

---

## 🧩 Verwendung eines Blueprints

1. **Neue Automation erstellen**
2. **„Aus Blueprint erstellen“** auswählen
3. Gewünschten Blueprint auswählen
4. Felder im UI konfigurieren
5. Automation speichern

---

## 🌍 Mehrsprachigkeit (i18n)

Einige Blueprints unterstützen automatische Sprachumschaltung:

- Deutsch / Englisch
- Erkennung über die Home-Assistant-UI-Sprache
- automatische Auswahl der passenden Texte
- optional sprachabhängige TTS-Ausgabe

Details zur Sprachunterstützung sind im jeweiligen Blueprint beschrieben.

---

## 🔊 Text-to-Speech (TTS)

Je nach Blueprint werden optionale TTS-Funktionen unterstützt:

- Sprachausgabe über Media Player
- automatische Sprachwahl (z. B. DE / EN)
- kompatibel mit gängigen Home-Assistant-TTS-Integrationen
- Unterstützung mehrerer Zielgeräte

Die verfügbaren Optionen hängen von der verwendeten TTS-Integration ab.

---

## ⚠️ Hinweise

- Die Nutzung erfolgt **auf eigene Gefahr**
- Vor produktivem Einsatz wird ein Test empfohlen
- Schwellwerte (z. B. Leistung, Zeiten) sollten an das jeweilige Gerät angepasst werden

---

## 🛠️ Troubleshooting

**Blueprint wird nicht angezeigt**
- URL muss eine `raw.githubusercontent.com`-Adresse sein
- Datei muss auf `.yaml` enden
- Home Assistant ggf. neu laden

**Automation löst unerwartet aus**
- Schwellwerte überprüfen
- Hilfs-Entitäten (Helper) korrekt gesetzt?
- Zeitbedingungen ggf. erhöhen

---

## 📜 Lizenz

Dieses Projekt wird ohne Gewähr bereitgestellt.  
Die Nutzung, Anpassung und Weitergabe im privaten Umfeld ist gestattet.

---

## ✨ Versionierung

Jeder Blueprint enthält:
- eine Versionsnummer
- ein Änderungsdatum
- eine `source_url` zur Rückverfolgung

Änderungen werden über GitHub-Releases dokumentiert.
