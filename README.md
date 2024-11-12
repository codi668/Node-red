# Node-RED Installation auf Raspberry Pi

Diese Anleitung beschreibt die Schritte zur Installation und Einrichtung von [Node-RED](https://nodered.org) auf einem Raspberry Pi. Node-RED ist eine Flow-basierte Entwicklungsumgebung, die ideal für IoT- und Automatisierungsprojekte geeignet ist.

## Voraussetzungen

- **Raspberry Pi** mit installiertem Raspberry Pi OS (vorzugsweise die neueste Version).
- **Netzwerkverbindung** (WLAN oder Ethernet).
- **Zugang zu einem Terminal** oder SSH.

---

## Schritt 1: System aktualisieren

Zuerst sollte sichergestellt werden, dass das System auf dem neuesten Stand ist. Öffne ein Terminal und führe die folgenden Befehle aus:

```bash
sudo apt update
sudo apt upgrade -y
```
## Schritt 2: Node-RED Installationsskript ausführen

Node-RED bietet ein Installationsskript speziell für den Raspberry Pi, das alle notwendigen Abhängigkeiten und Node.js installiert. Um das Skript herunterzuladen und auszuführen, gib folgenden Befehl ein:

```bash
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
```
## Schritt 3: Node-RED als Dienst einrichten (optional)

Um Node-RED automatisch beim Systemstart zu starten, aktiviere den Dienst mit folgendem Befehl:

```bash
sudo systemctl enable nodered.service
```
