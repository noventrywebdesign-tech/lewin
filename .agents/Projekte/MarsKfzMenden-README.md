# M.A.R.S. Kfz-Service & Mietwerkstatt Menden – Relaunch-Konzept

Datei: `MarsKfzMenden.html` (eine Datei, kein Build). Assets: `assets/mars-kfz-menden/`.
Lokal starten: `cd .agents/Projekte && python3 -m http.server 8765` → http://127.0.0.1:8765/MarsKfzMenden.html

## Quellen der Unternehmensdaten (Stand 31.10.2026)
- mars-kfz-menden.de (Start, /services, /ueber-uns, /kontakt, /impressum, /datenschutz)
- Name laut Seitentitel: „M.A.R.S. Mietwerkstatt & Kfz-Service Temore“
- Adresse: Balver Straße 34, 58706 Menden (Sauerland). Die Kontaktseite schreibt einmal „58708“; überall sonst steht 58706, das wird verwendet.
- Telefon: 0151 46349229 / 02373 3991101 · E-Mail: kfz.mars.menden@web.de
- Öffnungszeiten (Kontaktseite): Mo–Fr 9–19 Uhr, Sa 8–16 Uhr

## Vor dem Livegang klären
1. **Impressum:** Das Impressum der bestehenden Website ist leer. Inhaber/in (vollständiger Name), Rechtsform und ggf. USt-IdNr. fehlen. Auf der Seite steht dazu ein sichtbarer Hinweis.
2. **Öffnungszeiten:** Eine Kleinanzeigen-Anzeige (ca. 6 Monate alt) nennt andere Zeiten: Di–Fr 9–19, Sa 8–16, Mo 14–17 nur DHL. Bitte beim Kunden bestätigen.
3. **DHL-Paketshop:** Das Örtliche führt „DHL Paketshop 481“ unter derselben Adresse. Das steht nicht auf der eigenen Website und ist deshalb nicht übernommen.
4. **Bewertungen:** Verzeichnisse zeigen 5,0 (werkenntdenbesten, 58 Bewertungen) bzw. 4,9★. Das ist nicht live auf Google geprüft und deshalb nicht eingebaut.
5. **Logo:** Das bisherige Logo ist eine Clip-Art-Grafik. Auf der Seite steht stattdessen eine typografische Wortmarke mit Planet-Symbol. Das Originallogo kann bei Bedarf ergänzt werden.
6. Das Kontaktformular öffnet das E-Mail-Programm (mailto) und hat kein Backend.

## Bild- und Videomaterial (Symbolbilder, frei nutzbar)
Videos (Pexels-Lizenz): Hero 6157968 (Pavel Danilyuk, Politur), Aufbereitung 6872088 (Felgenpflege). Beide Frame für Frame auf Markenlogos geprüft. Das zuerst gewählte Video 6159287 zeigte ein Bentley-Emblem und wurde ersetzt.
Fotos (Unsplash-Lizenz, keine Unsplash+-Bilder), lokal in 720/1400 px:
svc-kfz 1619642751034 · svc-oel 1784619588643 · svc-check 1728474751252 · svc-inspektion 1615906655593 · svc-reifen 1645445522156 · svc-einlagerung 1527266258038 · svc-tuev 1760317890314 · svc-aufbereitung 1780558852670 · svc-hebebuehne 1723099971299 · svc-teile 1537462715879 · miet-main 1676018366904 · miet-lift 1613214150132 · miet-tools 1637640125496 · auf-politur 1620584898989 · auf-innen 1771491237218 · auf-felgen 1708805282683 · auf-waesche 1694678505383 · why-bg 1567808291548 · about 1599256872237
Im Impressum steht ein Bildnachweis mit dem Hinweis, dass die Bilder nicht die Räume von M.A.R.S. zeigen.

## Technik
Fonts (Archivo variabel, JetBrains Mono), Bilder und Videos liegen lokal. Die Seite macht keine Requests an Dritte, Google Maps lädt erst nach Klick (2-Klick-Lösung).
Video-Auflösung je nach Viewport (720p/540p). Bei prefers-reduced-motion oder Save-Data läuft kein Video, dann erscheint das Poster.
JSON-LD `AutoRepair` mit Öffnungszeiten und Leistungskatalog.
