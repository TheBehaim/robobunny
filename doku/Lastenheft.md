# Lastenheft RoboBunny

## Überblick
Der RoboBunny ist ein autonomer Roboter in Zwergkaninchenform, der sich realistisch bewegt, auf Interaktionen reagiert und lernfähig ist. Hier werden die geplanten Funktionen kategorisiert.

---

## Muss-Funktionen (Basis)

| Feature                        | Beschreibung |
|-------------------------------|--------------|
| Hoppeln                       | Fortbewegung durch Sprung-Sequenzen mit 4 Beinen |
| Sitz-/Liegeposition           | Fähigkeit, aufrecht zu sitzen und eingerollt zu ruhen |
| Ohren-/Schwanzbewegung        | Ausdruck über bewegliche Ohren & wackelnden Schwanz |
| Nase wackeln                  | Charakteristisches Zucken per Mikro-Servo oder Vibration |
| Touch-Sensorik (Streicheln)   | Kapazitive Sensorik am Kopf und Rücken |
| Sprachaktivierung (Wakeword)  | Offline-Spracherkennung z. B. „Hoppel“ via Picovoice |
| Kamera-Input (z. B. Objekte)  | Objekterkennung via OpenCV & TFLite |
| Grund-KI Verhalten            | Gaitsteuerung, Interaktion, Zufallsverhalten, States |
| Akku & Steuerung              | 3S LiPo, Raspberry Pi 5, DC/DC-Versorgung, Sicherheit |
| Notfall-Abschaltung           | Soft- oder Hardwarebasierter Not-Aus |

---

## Soll-Funktionen (erweiterte Ziele)

| Feature                        | Beschreibung |
|-------------------------------|--------------|
| Gesichtserkennung             | Wiedererkennen bestimmter Personen (z. B. Besitzer) |
| Autonomes Herumlaufen         | Raum-Erkundung mit Hindernisvermeidung |
| Rückkehr zur Ladestation      | Optionale Dockingfunktion bei niedrigem Akkustand |
| Ausdruck durch Geräusche      | Mini-Lautsprecher zur nonverbalen Rückmeldung |
| Drucksensoren in Pfoten       | Erkennung von Bodenkontakt & Hochheben |
| Gait-Simulation in PyBullet   | Vorab-Test der Gangalgorithmen |
| Watchdog-MCU (Failsafe)       | Arduino/ESP zur Überwachung & Notstopp |
| Py-Webinterface zur Telemetrie| Anzeige von Sensorwerten über Browser |
| LiDAR (z. B. TF-Luna)         | Tiefenerkennung & präzise Navigation |
| Kamera-Gimbal                 | Aktive Kopfbewegung zur Zielverfolgung |
| Simulation (PyBullet)         | Digitale Umgebung zur Gait-Planung & Debugging |

---

## Kann-Funktionen (später oder optional)

| Feature                        | Beschreibung |
|-------------------------------|--------------|

| ROS 2 Integration             | Modulare Architektur mit Nodes und Visualisierung |
| Bluetooth Fernwartung         | Kommunikation mit Handy/PC über BT |
| LED-Augen/Statusanzeigen      | Emotionen oder Status visuell darstellen |
| Reinforcement Learning        | Lernen durch Belohnung (z. B. Streicheln) |
| Verhaltenstrainer (Unity GUI)| C#-basierte Desktop-App zur Bewegungsprogrammierung |

---

## Sonstige Ideen

| Demo-Loop                     | Hase zeigt alle Tricks (Hoppeln, Ohren, Schwänzchen) auf Knopfdruck – gut für Vorführungen |
| Schüchternheits-Gradient      | Fremde Personen zuerst vorsichtig anpirschen; reagiert stärker, sobald Besitzer in der Nähe ist |
| Social Zone                   | Hase bleibt in vordefiniertem Bereich (z. B. Wohnzimmer), um Gäste nicht zu stören |

## Zeit & Budgetrahmen

- **Gesamtbudget:** max. 5.000 €
- **Zielkosten Basisversion:** ca. 2.500–3.000 €
- **Geplante Dauer:** ca. 2 Jahre mit 5 Phasen (siehe Projektplan)

---

## Nächster Schritt

→ Abgleich mit CAD: Alle *MUSS- und SOLL*-Funktionen müssen in Block-Out (z. B. Kameraöffnung, IMU-Position, Platz für Servo IDs) eingeplant sein.
