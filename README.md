# PowerDot-fw

Öffentliche Firmware-Releases für **PowerDot** (.bin-OTA-Assets).
Der Quellcode bleibt privat.

Das Gerät prüft über die GitHub-Release-API automatisch auf neue Versionen
und installiert sie auf Knopfdruck (Web-UI → Firmware-Update).

---

## Changelog

### In Arbeit (noch nicht veröffentlicht)
- Online-Update direkt über GitHub (Versionsprüfung + Ein-Klick-Installation)
- Live-Versionsanzeige aus dem neuesten GitHub-Release
- Update-Fortschritt als Vollbild-Anzeige am Gerät und in der Web-UI
- Firmware-Version in den Dot-Untereinstellungen sichtbar
- Auto-Reset der Arc-Maximalwerte: nie / täglich / wöchentlich / monatlich
- Splash-Screen mit doppeltem, gegenläufig pulsierendem Ring
- Drag-&-Drop-Fix beim manuellen Firmware-Upload

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
