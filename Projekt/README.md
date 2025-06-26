# LB Projekt M347 - Containerisierte Dienste

## Übersicht

Voraussetzungen:
- Internetverbindung
- Ubuntu 24.04 (DESKTOP VERSION mit GUI)
- Browser in der Ubuntu Umgebung

Dieses Projekt enthält folgende containerisierte Dienste:

- Wordpress (Port 8080)
- MediaWiki (Port 8181)
- Jira (Port 8081)
- Portainer (Port 9000)

## Installation

1. In Ubuntu Desktop Terminal öffnen und mit Schritt 2 fortfahren

2. Repository clonen:
    ```bash
    git clone https://github.com/Svensemann93/LB-Projekt-M347.git
    cd LB-Projekt-M347/Projekt
    ```
3. Ordnerstruktur im Ubuntu prüfen, nachdem das Repository gecloned wurde.

4. In den jeweiligen Ordner vom Service wechseln, z.B. Wordpress oder Portainer wechseln und dort das Terminal in diesem Ordner öffnen. Danach für jeden Service den folgenden Befehl ausführen. Weitere Details sind in den .html files zu finden.
    ```bash
    docker compose up -d
    ```

5. Dienste im Browser testen. (http://localhost:8080 bei Wordpress z.B.), für andere Dienste die unten aufgeführten Ports verwenden. 

6. Weitere Informationen sind in folgenden Dokumenten zu finden: (Falls das README.md nicht ausreicht)

Folgende Reihenfolge der Dokumente gilt es zu beachten:
- INFRASTRUKTUR.html
- KONFIGURATION.html
- INSTALLATION.html

7. Anhänge

- Hilfestellung und Quellen: HILFESTELLUNG.html
- Testplan für Persistenztest: TESTPLAN.html
- Abschlussplan vom Projekt mit Zusammenfasssung: ABSCHLUSSPLAN.html

## Stacks

| Dienst      | Port |
|-------------|------|
| Wordpress   | 8080 |
| MediaWiki   | 8181 |
| Portainer   | 9000 |
| Jira        | 8081 |

## Hinweise

- Ports müssen auf dem Host freigegeben und nicht besetzt sein!
