
## 🚁 Projekt: DIY-Drohne

Entwicklung und Bau einer eigenen Quadrocopter-Drohne mit selbst entwickelter Hardware und Software.

Ziel ist es, möglichst viele Komponenten selbst zu entwickeln und dabei Erfahrungen in den Bereichen Embedded Systems, Regelungstechnik, PCB-Design und Echtzeitsysteme zu sammeln.

### 📋 Projektübersicht

| Eigenschaft | Planung |
| :--- | :--- |
| **Budget** | Ca. 50 € |
| **Gewicht** | Max. 250 g |
| **Größe** | Ca. 12 × 12 cm (vorläufig) |
| **Bauform** | Quadrocopter (4 Motoren) |
| **Programmiersprachen** | C, C++ oder Rust |
| **Entwicklungsumgebung** | VS Code / weitere IDEs |
| **PCB-Design** | KiCad |
| **CAD-Konstruktion** | Fusion 360 / Alternativen |
| **Projektstatus** | 🟡 Konzeptphase |

---

### 🔧 Hardware

Folgende Komponenten werden voraussichtlich benötigt:

- [ ] 4 × Elektromotoren
- [ ] Motoransteuerung (ESCs oder eigene Treiberschaltung)
- [ ] Mikrocontroller oder Raspberry Pi
- [ ] IMU (Beschleunigungssensor und Gyroskop)
- [ ] Barometer zur Höhenmessung
- [ ] Akku und Spannungsversorgung
- [ ] Eigene Platine (PCB)
- [ ] Drohnenrahmen
- [ ] Propeller
- [ ] Optional: Kamera
- [ ] Optional: Funkmodul

**Offene Hardwarefragen:**
- Welcher Mikrocontroller eignet sich am besten?
- Raspberry Pi oder Mikrocontroller als Hauptrechner?
- Welche Motoren und Propeller passen zur Drohnengröße?
- Wie lässt sich das Gewicht unter 250 g halten?
- Welche Komponenten können auf einer eigenen Platine integriert werden?

---

### 💻 Software & Regelungstechnik

#### Flugregelung
- Entwicklung einer eigenen Flugregelung
- Auswertung von IMU- und Barometerdaten
- Lageregelung (Roll, Pitch, Yaw)
- Optional: Höhenregelung
- Untersuchung verschiedener Regelungsansätze (z. B. PID)

#### Rapid Control Prototyping (RCP)
- Prüfen, ob RCP für die Reglerentwicklung sinnvoll ist
- Modellbasierte Entwicklung der Flugregelung
- Automatische Codegenerierung aus einem Reglermodell
- Integration des generierten Codes auf dem Mikrocontroller

#### Echtzeitsystem (RTOS)
- Prüfung des Einsatzes eines RTOS
- Zeitgesteuerte Ausführung der Regelalgorithmen
- Sensorabfrage und Datenverarbeitung
- Kommunikation zwischen verschiedenen Softwaretasks

#### Kommunikation
- Entscheidung zwischen autonomem/lokalem Betrieb und Funksteuerung
- Optional: Drahtlose Übertragung von Messdaten
- Optional: Kameraübertragung
- Entwicklung eines geeigneten Kommunikationskonzepts

---

### 🛠️ Entwicklungswerkzeuge

| Bereich | Werkzeug |
| :--- | :--- |
| Firmware | C / C++ / Rust |
| IDE | Visual Studio Code |
| PCB-Design | KiCad |
| CAD | Fusion 360 |
| Regelungsentwicklung | MATLAB / Simulink (optional) |
| Versionsverwaltung | Git / GitHub |

---

### 👥 Aufgabenverteilung

| Person | Schwerpunkt | Aufgaben |
| :--- | :--- | :--- |
| **Marcus** | Kamera & Recheneinheit | Kamerakonzept, Raspberry Pi oder Mikrocontroller evaluieren |
| **Nicholas** | Regelungstechnik | Flugregelung, RCP und automatische Codegenerierung untersuchen |
| **Nico** | Embedded Software & Sensorik | RTOS-Konzept, Sensorauswahl und Sensoranbindung untersuchen |

#### Marcus – Kamera & Recheneinheit
- [ ] Möglichkeiten zur Kameraintegration untersuchen
- [ ] Raspberry Pi und Mikrocontroller vergleichen
- [ ] Anforderungen an Rechenleistung und Energieverbrauch bestimmen
- [ ] Erste Hardwareempfehlung erarbeiten

#### Nicholas – Regelungstechnik
- [ ] Grundlagen der Drohnenregelung untersuchen
- [ ] Geeignete Regelungsstruktur erarbeiten
- [ ] Einsatzmöglichkeiten von RCP prüfen
- [ ] Automatische Codegenerierung evaluieren
- [ ] Anforderungen an die Reglerausführung definieren

#### Nico – RTOS & Sensorik
- [ ] Geeignete IMU-Sensoren vergleichen
- [ ] Barometer und weitere Sensoren untersuchen
- [ ] RTOS gegenüber einer Bare-Metal-Lösung bewerten
- [ ] Sensoranbindung über I²C / SPI untersuchen
- [ ] Konzept für Sensorabfrage und zeitgesteuerte Verarbeitung erarbeiten

---

### ❓ Offene Entscheidungen

- [ ] Endgültige Größe und Gewicht festlegen
- [ ] Budget und Kostenaufteilung konkretisieren
- [ ] Mikrocontroller / Recheneinheit auswählen
- [ ] Motoren, Propeller und Akku auswählen
- [ ] Programmiersprache festlegen
- [ ] RTOS oder Bare Metal entscheiden
- [ ] Einsatz von RCP und Codegenerierung festlegen
- [ ] Kamera ja/nein entscheiden
- [ ] Funksteuerung oder lokaler/autonomer Betrieb entscheiden
- [ ] Erste Systemarchitektur erstellen

---

### 🗺️ Geplanter Projektablauf

| Phase | Inhalt | Status |
| :--- | :--- | :--- |
| 1. Konzept | Anforderungen, Recherche und Aufgabenverteilung | 🟡 In Arbeit |
| 2. Hardwareauswahl | Motoren, Sensoren, Akku und Mikrocontroller | ⚪ Offen |
| 3. Systemdesign | Schaltplan, PCB und CAD-Modell | ⚪ Offen |
| 4. Softwareentwicklung | Sensorik, RTOS und Flugregelung | ⚪ Offen |
| 5. Integration | Zusammenbau und Inbetriebnahme | ⚪ Offen |
| 6. Tests | Reglertuning, Prüfstand und Flugversuche | ⚪ Offen |

---

### 🎯 Erstes gemeinsames Ziel

Erstellung eines grundlegenden Systemkonzepts mit:

1. Grober Hardwarearchitektur
2. Vorauswahl der wichtigsten Komponenten
3. Konzept für Software und Flugregelung
4. Erste Kostenschätzung
5. Entscheidung über das weitere Vorgehen
