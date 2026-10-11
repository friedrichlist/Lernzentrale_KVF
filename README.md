# Lernzentrale KVF

Training und Prüfungsvorbereitung für alle drei Ausbildungsjahre der Kaufleute für Versicherungen und Finanzanlagen an der BbS IV „Friedrich List“ Halle (Saale): Startseite mit Prüfungspass je Klasse, Prüfungstrainings (GAP 1, GAP 2 Teil 1.1 und Teil 1.2 je Sparte, später WISO) und je Lernsituation ein Modul als einzelne HTML-Datei.

**Live:** https://friedrichlist.github.io/Lernzentrale_KVF/ (bis 10.10.2026: `Lernzentrale_2AJ_KVF`)

Der Lernstand bleibt im Browser des jeweiligen Geräts. Kein Backend, keine Anmeldung, keine Datenübertragung. Die Startseite funktioniert nur, wenn alle Seiten in diesem Repository liegen (gleiche Adresse = gemeinsamer Browserspeicher). Die Auswertung der Meldecodes ist nur für die Lehrkraft und wird hier nicht hochgeladen.

| Datei | Zweck |
|---|---|
| `index.html` | Startseite: Klassenwahl, Prüfungen der Klasse mit Terminen, Prüfungspass (Trainingspunkte, Prüfungsreife), Module, Klassen-Challenge – gebaut mit `bau_pass.py` |
| `KVF_LF06_LS06.1_Lernzentrale.html` | LF 6 · LS 06.1 „Kfz versichern – die Kundenakte Brehmer“ (TE 1–5) |
| `GAP1_Pruefungstraining.html` | Prüfungstraining GAP 1 (6 Prüfungsbereiche, 617 Aufgaben mit Rechenwerkstatt Wohnen, Simulation) |
| `GAP2_T11_Pruefungstraining.html` | Prüfungstraining GAP 2 Teil 1.1 (5 Prüfungsaufgaben, 192 Aufgaben in der Hauptrunde + 167 in der Zusatzrunde, Simulation) – im Pass sichtbar ab dem Monat nach der GAP 1 der Klasse |
| `GAP2_T12_Wohnen.html`, `GAP2_T12_Beruf_und_Freizeit.html`, `GAP2_T12_Mobilitaet_und_Reisen.html`, `GAP2_T12_Einkommen_und_Hinterbliebene.html`, `GAP2_T12_Gesundheit_und_Pflege.html`, `GAP2_T12_Vorsorge.html` | Prüfungstraining GAP 2 Teil 1.2, je Sparte 56 Aufgaben mit Simulation. Im Pass wählt jede/r die eigene Sparte (ab drei Monate vor GAP 2); Gesundheit und Pflege mit Rechtsstand 01.01.2026 |
| `pruefungspass.html` | Weiterleitung auf `index.html` (für Links aus den Modulen) |
| `datenschutz.html` | Datenschutzhinweis – gebaut mit `bau_pass.py` |
| `icon-180.png`, `icon-192.png`, `icon-512.png` | App-Symbol (Icon der Listschule) für „Zum Home-Bildschirm“ |

Mein KVF verlinkt mit `index.html?klasse=KVF26` (Klassenkennung); die Startseite merkt sich die Klasse.

Gestaltung im Corporate Design der Listschule Halle (Saale): Farben, Logo und Icon nach dem Design Manual, Schrift Montserrat (SIL Open Font License 1.1, Copyright 2011 The Montserrat Project Authors) in die Seiten eingebettet – es werden keine Schriften von anderen Anbietern geladen.

## Neue Fassung einspielen

Die Module werden im OneDrive unter `KVF/Interaktive Lernzentrale` gebaut (`Werkzeug/bau_lz.py`, `Werkzeug/pass/bau_pass.py`, Daten in `Daten/`). Hier wird nur die fertige
Datei aus `Module/` hochgeladen (nie `Module/Pruefungspass/Lehrkraft/`) – nie `Daten/`, `Werkzeug/` oder `Berichte/`. Nach dem Hochladen dauert es ein bis zwei Minuten, bis GitHub Pages
die neue Fassung ausliefert.
