# PowerDot-fw

Oeffentliche Firmware-Releases fuer **PowerDot** (.bin-OTA-Assets).
Der Quellcode bleibt privat.

Das Geraet prueft ueber die GitHub-Release-API automatisch auf neue Versionen
und installiert sie auf Knopfdruck (Web-UI Firmware-Update).

---

## Changelog

### v2.0.4-beta - 2026-06-27

**Neu**
- "MQTT nicht verbunden"-Screen: das Display zeigt klar an, wenn der Cerbo konfiguriert, MQTT aber getrennt ist (inkl. Kurzanleitung) - verschwindet automatisch bei Verbindung
- Setup-Assistent: neuer 3. Schritt "MQTT aktivieren" (Einstellungen -> Integrationen -> MQTT-Zugang)
- Hotspot-Name kontextabhaengig: "PowerDot Einrichtung" bei der Ersteinrichtung, "PowerDot Web UI" beim manuell gestarteten Hotspot

**Behoben**
- Kein periodisches Einfrieren mehr bei nicht erreichbarem Cerbo/MQTT (nicht-blockierender TCP-Probe statt blockierendem Connect)
- Splash-Haenger behoben: MQTT-Connect laeuft jetzt unsichtbar in der Splash-Animation
- Setup-Assistent: "Verbinden"-Button und WLAN-Auswahl funktionierten nicht (defektes JavaScript) - behoben

---

### v2.0.3-beta - 2026-06-23

**Behoben**
- Autoscroll/Timeout/Helligkeit-Wert wird nach Neustart korrekt wiederhergestellt (NVS-Debounce entfernt)
- OTA-Updatepruefung funktioniert jetzt auch mit Beta-Releases (HTTP 404 behoben)
- Werksreset-Arc bricht nicht mehr vorzeitig ab beim 5s-Halten (PRESS_LOST-Fehlausloeser entfernt)
- WiFi-Setup: Eingabefelder heller und besser sichtbar

---

### v2.0.2-beta - 2026-06-18

**Behoben**
- Autoscroll-Wert ging nach Stromtrennung verloren - finaler Arc-Wert wird beim Loslassen immer in NVS gespeichert
- Multi RS Solar: integrierter MPPT wurde in Solar-Werten nicht erkannt - MQTT-Topics vebus/Pv/0/P + Pv/1/P werden jetzt erfasst

**Neu**
- Seiteneinstellungen: Listenelemente folgen beim Scrollen der Kreiskruemmung des runden Displays

---

### v2.0.1-beta - 2026-06-13

**Neu**
- Online-Update direkt ueber GitHub (Versionspruefung + Ein-Klick-Installation)
- Live-Versionsanzeige aus dem neuesten GitHub-Release
- Update-Fortschritt als Vollbild-Anzeige am Geraet und in der Web-UI
- Firmware-Version in den Dot-Untereinstellungen sichtbar
- Auto-Reset der Arc-Maximalwerte: nie / taeglich / woechentlich / monatlich
- Splash-Screen mit doppeltem, gegenlaeufig pulsierendem Ring

**Behoben**
- Werksreset ueber die Web-UI loescht jetzt auch die Solar-Ertrags-Baseline
- Werksreset am Geraet (5s halten) bouncte beim Antippen - Touch-Settling wird toleriert
- Drag-and-Drop beim manuellen Firmware-Upload
- Update-Pruefung vergleicht Versionen jetzt semantisch (kein versehentliches Downgrade-Angebot)

---

### v2.0.0-beta - 2026-06-12
- Erste oeffentliche Release-Version
- Victron-Energieueberwachung (Batterie, Solar, Netz, Lasten, EVCS)
- Uebersicht mit Peak-Hold-Arcs
- WLAN-Setup ueber temporaeren Access-Point
- Web-Oberflaeche fuer Einstellungen und Firmware-Update
- PCM5101-I2S-Audio (Bestaetigungs-Sounds)

---

> Hinweis: Die automatisch angehaengte Source code zip enthaelt nur dieses README, nicht den privaten Firmware-Quellcode.
