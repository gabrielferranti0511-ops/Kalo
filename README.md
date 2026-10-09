# Kalo

Kalo ist ein Kalorien-Tracker für das Handy. Du trägst Mahlzeiten ein und siehst Tagesziel, Defizit, Wasser, Gewicht und Verlauf. Die App besteht aus einer Seite (`index.html`), ohne Framework und ohne Build-Schritt.

## Dateien

| Datei | Wofür |
|---|---|
| `index.html` | die ganze App |
| `favicon.svg` | Symbol im Browser-Tab |
| `favicon-32.png` | Symbol im Tab für ältere Browser |
| `apple-touch-icon.png` | Symbol auf dem iPhone-Home-Bildschirm (180 × 180) |
| `icon-192.png`, `icon-512.png` | Symbole für Android und die App-Installation |
| `site.webmanifest` | Name, Farben und Symbole für „Zum Home-Bildschirm“ |
| `README.md` | diese Beschreibung |

Alle Dateien liegen im Hauptordner des Repositorys, nicht in einem Unterordner.

## Funktionen

- Einrichtungs-Assistent mit Berechnung von Grundumsatz, Gesamtumsatz, Tagesziel und Defizit
- Großer Ring, der Kalorien, Bedarf, Tageszeit oder Defizit zeigt, dazu Nährwert-Ringe
- Tagebuch nach Mahlzeiten, Bearbeiten und Löschen, Favoriten, Kopieren von anderen Tagen
- Wasser, Sport, Fasten-Timer, Befinden, weitere Nährwerte
- Plan für Woche, Monat und Jahr, Kalender, Wochenbalken, Serie und Abzeichen
- Gewichtskurve mit Prognose, Wochenziele
- Spruch des Tages

## Was auf GitHub Pages nicht geht

Foto-Scan, Text-Schätzung, Rezept-Berechnung, Sport-Schätzung, Wochenplaner, Auswertung, Speichern im Konto und die Export-Knöpfe brauchen die Verbindung zu Claude. Sie laufen nur, wenn die Seite als Claude-Artifact geöffnet wird. Auf GitHub speichert die App im Browser des Geräts (`localStorage`). Mahlzeiten trägst du dort von Hand ein.

## Veröffentlichen mit GitHub Pages

1. Lege auf github.com ein neues **öffentliches** Repository an, zum Beispiel `kalo`.
2. Lade **alle Dateien** aus der Tabelle oben hoch (**Add file → Upload files**, alle gleichzeitig hineinziehen).
3. Klicke auf **Commit changes**.
4. Gehe zu **Settings → Pages**, wähle **Deploy from a branch**, Branch `main`, Ordner `/ (root)`, und klicke auf **Save**.
5. Nach ein bis zwei Minuten läuft die Seite unter `https://DEINNAME.github.io/kalo/`.

Den Fortschritt siehst du im Reiter **Actions** (grüner Haken = fertig).

## Auf den Home-Bildschirm legen

**iPhone (Safari):** Seite öffnen, unten auf **Teilen** tippen, dann **Zum Home-Bildschirm**. Das Kalo-Symbol erscheint auf deinem Bildschirm, und die Seite öffnet sich ohne Browser-Leiste.

**Android (Chrome):** Menü mit den drei Punkten, dann **App installieren** oder **Zum Startbildschirm**.

Hast du die Seite schon vorher hinzugefügt und siehst noch das alte Symbol, lösche sie vom Home-Bildschirm und füge sie neu hinzu. Browser merken sich Symbole sehr lange. Für den Tab hilft ein harter Neustart der Seite oder ein neuer Tab.

## Wenn es nicht klappt

| Problem | Lösung |
|---|---|
| „404“ | Die Datei muss genau `index.html` heißen und im Hauptordner liegen. |
| Unter „Pages“ gibt es keine Einstellung | Das Repository ist privat. Stelle es unter Settings → General → Danger Zone → Change visibility auf Public. |
| Alte Version oder leere Seite | Zwei Minuten warten, dann neu laden. |
| Tab zeigt noch den Globus | Alle Symbol-Dateien hochladen (Tabelle oben) und den Tab neu öffnen. |
| Seite sieht winzig aus | Du hast eine alte `index.html` hochgeladen. Nimm die aktuelle Datei. |

## Hinweis

Kalo ersetzt keine ärztliche oder ernährungsberaterische Beratung. Die Werte sind Richtwerte. Bei Vorerkrankungen oder Schwangerschaft sprich vorher mit einer Ärztin oder einem Arzt.
