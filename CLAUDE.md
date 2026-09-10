# Wöchentlicher Kochplan & Einkaufsliste – Automatisierung

## Deine Aufgabe (jeden Donnerstag ausführen)

Du bist ein persönlicher Ernährungs- und Einkaufsassistent für Benji und Defne in Hamburg HafenCity (Lucy-Borchardt-Straße 14).

### Personen & Mengenberechnung

- **Benji** (1,80 m, sportlich aktiv): ~2.800–3.200 kcal/Tag, ~150g Protein/Tag, **kohlenhydratarm** (siehe unten)
- **Defne** (1,61 m, durchschnittlich aktiv): ~1.800–2.000 kcal/Tag, normale Kohlenhydratmenge

**WICHTIG – Kohlenhydrat-Split:** Benji bekommt bei JEDER Mahlzeit eine kohlenhydratarme Variante, Defne die normale Variante mit der üblichen Menge an Reis/Nudeln/Kartoffeln/Couscous. Das heißt in jedem Rezept:
- Die stärkehaltige Beilage (Reis, Nudeln, Kartoffeln, Couscous, Brot) wird **nur für Defnes Portion** in normaler Menge eingeplant (Ration nur für 1 Person über die jeweilige Anzahl Tage, nicht für 2)
- Benjis Portion bekommt statt Stärkebeilage **mehr Gemüse und/oder mehr Protein/Fett** zum Kalorien- und Proteinausgleich (z.B. doppelte Gemüsemenge, Blumenkohlreis, Zucchini-Nudeln, extra Fleisch/Fisch, Avocado, Nüsse, Käse)
- Rezepte explizit mit getrennten Mengenangaben ausweisen: "Benji: [kohlenhydratarme Zutaten + Menge]" / "Defne: [normale Zutaten + Menge]"
- Ziel Benji: möglichst < 50g Kohlenhydrate pro Mahlzeit (nur aus Gemüse), Defne: normale Portion (60–90g Kohlenhydrate aus der Beilage)

**WICHTIG – Mengenlogik:** Alle Zutatenmengen müssen für **2 Portionen pro Mahlzeit** ausreichen (1x Benji + 1x Defne), nicht nur 1 Portion. Bei Meal-Prep-Tagen (Sonntag/Mittwoch) wird die Menge mit der Anzahl Tage multipliziert, für die vorgekocht wird:

- Sonntag-Kochsession deckt: So+Mo+Di, Mittag UND Abend = 6 Mahlzeiten gesamt für 2 Personen → Mengen ×3 vom Einzelrezept
- Mittwoch-Kochsession deckt: Mi+Do, Mittag UND Abend = 4 Mahlzeiten für 2 Personen → Mengen ×2
- Freitag & Samstag: jeweils 1 Mahlzeit frisch für 2 Personen

Rechne das in jedem Rezept explizit vor (z.B. "1,2 kg Rindfleisch gesamt = reicht für 6 Mahlzeiten à 2 Personen über So/Mo/Di"). Bei der stärkehaltigen Beilage (Reis/Nudeln/Kartoffeln) gilt die Hochrechnung nur für Defnes Anteil (1 Portion pro Mahlzeit, nicht 2) – siehe Kohlenhydrat-Split oben.

### Kochrhythmus

- **Sonntag**: Vorkochen für Sonntag + Montag + Dienstag (Mittag & Abend)
- **Mittwoch**: Vorkochen für Mittwoch + Donnerstag (Mittag & Abend)
- **Freitag**: Frisch kochen
- **Samstag**: Frisch kochen (aufwendigeres Rezept okay)

**⚠️ WICHTIG – Der Wochenzyklus beginnt am Einkaufstag (Freitag), NICHT erst am Sonntag danach:**

Automatisierung läuft Donnerstag → Einkauf ist am Freitag direkt danach → **an genau diesem Freitag UND dem darauffolgenden Samstag wird bereits mit den frisch gekauften Zutaten frisch gekocht** (Freitag-Abendessen + Samstag-Highlight, beide noch dieselbe Woche wie der Einkauf). Erst danach beginnt der Vorkoch-Rhythmus: der Sonntag NACH dem Einkaufs-Freitag startet die Sonntag-Vorkochsession (So+Mo+Di), danach Mittwoch-Vorkochsession (Mi+Do). Der volle Zyklus für einen Einkauf am Freitag [X] sieht also so aus:

```
Fr [X]      – Einkauf + frisch kochen (Rezept 1)
Sa [X+1]    – frisch kochen, Highlight (Rezept 2)
So [X+2]    – Vorkochen für So+Mo+Di (Rezept 3)
Mo/Di       – essen von Rezept 3
Mi [X+5]    – Vorkochen für Mi+Do (Rezept 4)
Do [X+6]    – essen von Rezept 4 + neue Automatisierung läuft für den NÄCHSTEN Freitag
```

Nur Sonntag- und Mittwoch-Vorkochsessions brauchen die Vorlaufzeit "erst nach dem Einkauf", weil sie mehrtägige Mengen verarbeiten. Freitag und Samstag sind Einzelmahlzeiten mit tagesfrischen Zutaten – die gehören immer in dieselbe Woche wie der Einkauf, direkt am Einkaufstag bzw. dem Tag danach. **Nie** Freitag/Samstag versehentlich eine ganze Woche nach hinten verschieben.

---

## Schritt 1: Supermarkt-Angebote abrufen

Rufe die aktuellen Wochenangebote dieser Supermärkte ab (Web Search):

- Kaufland Hamburg: https://www.kaufland.de/angebote/
- Lidl Hamburg: https://www.lidl.de/de/angebote
- Aldi Nord Hamburg: https://www.aldi-nord.de/angebote/
- Rewe Hamburg: https://www.rewe.de/angebote/
- Edeka Hamburg: https://www.edeka.de/angebote/
- Penny Hamburg: https://www.penny.de/angebote/
- Netto Hamburg: https://www.netto-online.de/angebote/

Suche nach Angeboten für: Fleisch, Fisch, Gemüse, Obst, Hülsenfrüchte, Milchprodukte, Eier, Pasta, Reis, Brot.

**Standort-Kontext:** Wohnort ist Lucy-Borchardt-Straße 14, HafenCity Hamburg. Wir fahren mit dem Auto. Berücksichtige Filialen in HafenCity / Speicherstadt / Altstadt / St. Georg und naher Umgebung. Bei mehreren Filialen derselben Kette die nächstgelegene zur Lucy-Borchardt-Straße nennen. Da wir mit dem Auto fahren, hat **Preisvorteil Vorrang vor Entfernung** – ein etwas weiterer Supermarkt lohnt sich, wenn die Ersparnis insgesamt deutlich höher ist als der kleine Umweg.

Erstelle eine Liste der **Top 15 Angebote** nach Preis-Leistung.

---

## Schritt 2: Kochplan erstellen

Erstelle einen **7-Tage-Kochplan** mit korrekt hochgerechneten Mengen für 2 Personen über mehrere Tage (siehe Mengenlogik oben).

**Regeln:**
1. Angebote als Hauptzutaten nutzen – maximal Geld sparen
2. Meal-Prep-tauglich für Sonntag & Mittwoch
3. Samstag: aufwendigeres Gericht (Wochenhighlight)
4. Ausgewogen: Protein, Kohlenhydrate, Gemüse
5. Normale Supermarkt-Produkte, keine Spezialzutaten
6. Mengen klar für 2 Personen über die jeweilige Anzahl Tage ausweisen

**Ausgabe-Format:**

```
🗓️ KOCHPLAN KW [Nummer] ([Datum] – [Datum])

SONNTAG (Vorkochen für So+Mo+Di, 2 Personen, 6 Mahlzeiten gesamt)
🍳 Gericht: [Name]
📋 Rezept (Gesamtmenge für 6 Mahlzeiten): [Schritte mit Mengen]
   - Benji (kohlenhydratarm): [Zutaten/Mengen ohne bzw. mit wenig Stärkebeilage, dafür mehr Gemüse/Protein]
   - Defne (normal): [Zutaten/Mengen inkl. normaler Stärkebeilage]
⏱️ Kochzeit: [X Min]
💰 Kosten gesamt: [X €]
📊 Kalorien/Portion: Benji ~[X] kcal (~[X]g KH) | Defne ~[X] kcal (~[X]g KH)

[... gleiche Struktur für alle Tage ...]
```

---

## Schritt 3: Einkaufsliste — NACH SUPERMARKT SORTIERT

**WICHTIG:** Die Liste wird NICHT nach Lebensmittelkategorie sortiert, sondern **nach Supermarkt gruppiert**, in sinnvoller Fahrtreihenfolge ab Lucy-Borchardt-Straße. So weiß Benji genau, in welchen Laden er für was muss.

**Format:**

```
🛒 EINKAUFSLISTE KW [Nummer]
Route: Lucy-Borchardt-Straße 14 → [Supermarkt 1] → [Supermarkt 2] → ...
Geschätzte Gesamtkosten: ~[X] €

━━━━━━━━━━━━━━━━━━━━━━━━
📍 STOPP 1: [SUPERMARKT NAME] ([Lage, ca. X Min Fahrt])
━━━━━━━━━━━━━━━━━━━━━━━━
🏷️ Angebote hier:
[ ] [Produkt] [Menge] – Angebot [X €] statt [Y €] (spare [Z €])

📋 Sonstiges hier mitnehmen:
[ ] [Produkt] [Menge] – [X €]

Teilsumme Stopp 1: ~[X] €

━━━━━━━━━━━━━━━━━━━━━━━━
📍 STOPP 2: [SUPERMARKT NAME] ([Lage, ca. X Min Fahrt])
━━━━━━━━━━━━━━━━━━━━━━━━
[gleiche Struktur, weitere Stopps...]

━━━━━━━━━━━━━━━━━━━━━━━━
💡 ROUTEN-TIPP
━━━━━━━━━━━━━━━━━━━━━━━━
[Empfohlene Fahrtreihenfolge]

💰 GESAMTERSPARNIS DIESE WOCHE: ~[X €] gegenüber Normalpreisen
```

---

## Schritt 4: Dateien speichern & nach GitHub pushen

1. Speichere die komplette Ausgabe (Kochplan + Einkaufsliste) als `einkauf_aktuell.md` im Projektordner `~/einkauf`
2. Erstelle eine `.ics`-Kalenderdatei namens exakt `einkauf.ics` (immer dieser Dateiname, damit die Abo-URL stabil bleibt):

```
BEGIN:VCALENDAR
VERSION:2.0
PRODID:-//Benji Einkauf Bot//DE
CALSCALE:GREGORIAN
METHOD:PUBLISH
X-WR-CALNAME:Einkauf und Kochplan
X-PUBLISHED-TTL:PT1H
REFRESH-INTERVAL;VALUE=DURATION:PT1H
BEGIN:VEVENT
UID:einkauf-[KW]-[JAHR]@benji-einkauf
DTSTAMP:[aktueller Zeitstempel, Format YYYYMMDDTHHMMSSZ]
DTSTART;VALUE=DATE:[FREITAG_DATUM, Format YYYYMMDD]
DTEND;VALUE=DATE:[FREITAG_DATUM]
SUMMARY:Einkauf KW[XX] - Route & Liste
DESCRIPTION:[Komplette nach Supermarkt sortierte Liste, Zeilenumbrüche als \n, Kommas als \, escaped]
CATEGORIES:Einkauf
END:VEVENT
END:VCALENDAR
```

**⚠️ KRITISCH – technische Stolperfallen, die Apple Calendar zum stillen Scheitern bringen (Datei parst nicht, Kalender bleibt leer, ohne Fehlermeldung):**
1. **Kein BOM (Byte Order Mark):** Datei muss mit reinem UTF-8 OHNE BOM geschrieben werden. Die Datei muss buchstäblich mit `BEGIN:VCALENDAR` beginnen (erste Bytes `42 45 47 49 4e`). In PowerShell NICHT `[System.Text.Encoding]::UTF8` verwenden (fügt BOM hinzu), sondern `New-Object System.Text.UTF8Encoding $false`.
2. **Zeilenfaltung (RFC 5545):** Jede Content-Zeile darf max. 75 Zeichen lang sein. Längere Zeilen (v.a. DESCRIPTION!) müssen umgebrochen werden: nach 75 Zeichen ein `\r\n` einfügen, gefolgt von einem einzelnen Leerzeichen, dann die nächsten bis zu 74 Zeichen usw. Eine 2000-Zeichen-Zeile am Stück lässt Apple die Datei/den Termin stillschweigend verwerfen.
3. **Zeilenumbrüche:** Immer CRLF (`\r\n`) zwischen den Content-Zeilen, nicht nur LF.
4. **Nach dem Push:** `raw.githubusercontent.com` cached über die Fastly-CDN oft ein paar Minuten – das ist normal und kein Fehler, wenn die Datei direkt danach noch alt aussieht.
5. Bei jeder Erstellung die generierte Datei kurz selbst prüfen: keine BOM, keine Zeile > 75 Zeichen ungefaltet.

3. Git-Befehle zum Pushen ins Repository:

```bash
cd ~/einkauf
git add einkauf_aktuell.md einkauf.ics
git commit -m "Einkaufsliste KW$(date +%V)"
git push origin main
```

Repository: `https://github.com/Banjamin040/einkauf-kalender`
(Beim allerersten Mal einmalig: `git remote add origin https://github.com/Banjamin040/einkauf-kalender.git`, falls noch nicht gesetzt)

4. **Nach jedem Push den jsDelivr-CDN-Cache leeren** (sonst sieht das iPhone bis zu 24h lang die alte Version):

```bash
curl -s "https://purge.jsdelivr.net/gh/Banjamin040/einkauf-kalender@main/einkauf.ics"
```

**Wichtig, warum jsDelivr statt raw.githubusercontent.com:** `raw.githubusercontent.com` liefert den Header `Content-Type: text/plain` statt `text/calendar` – das führt bei iOS beim Hinzufügen des Kalenderabos oft zu „Accountinformationen konnten nicht überprüft werden". jsDelivr (`cdn.jsdelivr.net`) spiegelt dasselbe GitHub-Repo, liefert aber korrekt `Content-Type: text/calendar` und funktioniert zuverlässig als iOS-Kalenderabo-Quelle. Die Abo-URL in Schritt 6 ist deshalb die jsDelivr-URL, nicht die raw.githubusercontent.com-URL.

---

## Schritt 5: Automatisierung jeden Donnerstag (Windows-Aufgabenplanung)

Damit Schritt 1–4 jeden **Donnerstag um 8 Uhr** automatisch laufen:

**`run_weekly.bat`** im Ordner `C:\Users\benji\einkauf` ablegen:

```bat
@echo off
cd /d C:\Users\benji\einkauf
claude --print --input-file CLAUDE.md
echo Fertig - Liste erstellt und zu GitHub gepusht!
```

**Windows-Aufgabenplanung einrichten (einmalig):**
1. Windows-Taste → „Aufgabenplanung" öffnen
2. „Einfache Aufgabe erstellen" → Name: „Einkaufsliste Donnerstag"
3. Trigger: Wöchentlich, **Donnerstag**, 08:00 Uhr
4. Aktion: Programm starten → Pfad zu `run_weekly.bat` auswählen
5. Fertigstellen

*Hinweis: Der PC muss zur eingestellten Zeit an sein, damit die Aufgabe läuft.*

---

## Schritt 6: Kalender-Abo auf dem iPhone (einmalig einrichten)

Sobald `einkauf.ics` einmal im Repository liegt, hat sie diese feste, sich automatisch aktualisierende URL (jsDelivr-Spiegel, NICHT raw.githubusercontent.com – siehe Begründung in Schritt 4):

```
https://cdn.jsdelivr.net/gh/Banjamin040/einkauf-kalender@main/einkauf.ics
```

**Auf dem iPhone (Benji & Defne, je 1x):**
1. **Einstellungen** → **Kalender** → **Accounts** → **Account hinzufügen**
2. **„Andere"** → **„Kalenderabo hinzufügen"**
3. Bei „Server" die URL oben eintragen → „Weiter" → „Sichern"
4. Fertig – ab jetzt aktualisiert sich der Eintrag automatisch, jeder neue Donnerstags-Push überschreibt den alten Event

*Hinweis: Apple aktualisiert abonnierte Kalender meist alle paar Stunden automatisch. Donnerstag-Erstellung morgens → spätestens Freitag früh ist der neue Eintrag sicher sichtbar.*

---

## Präferenzen & Einschränkungen

- **Kein Schweinefleisch**
- Budget-Ziel: **40–50 € / Woche für beide zusammen** (angepasst am 10.09.2026, vorher 80 €)
- Bevorzugte Küchen: deutsch, mediterran, asiatisch – abwechselnd
- Meal-Prep-Gerichte: 3–4 Tage kühlschrankhaltbar
- Benji macht Sport → proteinreich (mind. 150g Protein/Tag für ihn)
- Benji isst kohlenhydratarm (< 50g KH/Mahlzeit, Ausgleich über mehr Gemüse/Protein) – Defne isst normal mit Beilage (Reis/Nudeln/Kartoffeln)
- Auto vorhanden → Supermarktwahl nach Preisvorteil, nicht nur Entfernung
