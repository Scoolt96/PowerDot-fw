# PowerDot-fw

Öffentliche Firmware-Releases für **PowerDot** (.bin-OTA-Assets).
Der Quellcode bleibt privat.

Das Gerät prüft über die GitHub-Release-API automatisch auf neue Versionen
und installiert sie auf Knopfdruck (Web-UI → Firmware-Update).

---

## Changelog

### v2.0.1 — 2026-06-13
**Neu**
- Online-Update direkt über GitHub (Versionsprüfung + Ein-Klick-Installation)
- Live-Versionsanzeige aus dem neuesten GitHub-Release
- Update-Fortschritt als Vollbild-Anzeige am Gerät und in der Web-UI
- Firmware-Version in den Dot-Untereinstellungen sichtbar
- Auto-Reset der Arc-Maximalwerte: nie / täglich / wöchentlich / monatlich
- Splash-Screen mit doppeltem, gegenläufig pulsierendem Ring

**Behoben**
- Werksreset über die Web-UI löscht jetzt auch die Solar-Ertrags-Baseline (`solartd`)
- Werksreset am Gerät (5 s halten) bouncte beim Antippen — Touch-Settling wird toleriert
- Drag-&-Drop beim manuellen Firmware-Upload
- Update-Prüfung vergleicht Versionen jetzt semantisch (kein versehentliches Downgrade-Angebot)

### v2.0.0 — 2026-06-12
- Erste öffentliche Release-Version
- Victron-Energieüberwachung (Batterie, Solar, Netz, Lasten, EVCS)
- Übersicht mit Peak-Hold-Arcs
- WLAN-Setup über temporären Access-Point
- Web-Oberfläche für Einstellungen und Firmware-Update
- PCM5101-I2S-Audio (Bestätigungs-Sounds)

---

> Hinweis: Die automatisch angehängte „Source code (zip)" enthält nur dieses
> README, **nicht** den privaten Firmware-Quellcode.
