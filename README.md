# HabitHero – README für die Projektabgabe

## Online-Version

Die Web-App kann direkt über GitHub Pages geöffnet und getestet werden:

**https://haeusele83.github.io/habit_hero/**

Damit muss die Anwendung für die erste Sichtung nicht lokal installiert oder konfiguriert werden. Die App läuft direkt im Browser.

## Kurzbeschreibung

HabitHero ist eine einfache und motivierende Web-App zur Unterstützung beim Aufbau positiver Gewohnheiten. Nutzerinnen und Nutzer können persönliche Habits erfassen, täglich abhaken und ihren Fortschritt über ein übersichtliches Dashboard verfolgen. Ergänzend nutzt die App Gamification-Elemente wie XP, Level und Badges, um die Motivation langfristig zu erhöhen.

Die Anwendung wurde bewusst als schlanker MVP umgesetzt. Der Fokus liegt auf einer klaren Bedienung, einer stabilen lokalen Speicherung und einer überzeugenden Live-Demo im Browser.

## Technische Umsetzung

Die App wurde als statische Web-App mit HTML, CSS und JavaScript umgesetzt. Sie kann entweder direkt über GitHub Pages oder lokal über Visual Studio Code mit der Erweiterung Live Server gestartet werden. Es wird kein Backend, keine externe Datenbank und keine zusätzliche Build-Umgebung benötigt.

Die Daten werden lokal im Browser über `localStorage` gespeichert. Dadurch bleiben erfasste Habits auch nach dem Neuladen der Seite erhalten. Für die Demonstration können Demo-Daten geladen werden.


## Hinweis zu GitHub Pages und Assets

Die sichtbaren Logo-Grafiken sind in dieser Version zusätzlich direkt in `index.html` eingebettet. Dadurch werden Logo und Favicon auch dann angezeigt, wenn GitHub Pages Asset-Pfade sehr strikt auswertet oder einzelne Dateien nicht korrekt übertragen wurden. Der Ordner `assets/` bleibt trotzdem im Projekt enthalten, damit die Bilder weiterhin sauber dokumentiert und bei Bedarf separat austauschbar sind.

Wichtig beim Hochladen auf GitHub: Der Ordner `assets` muss vollständig mitgeführt werden. GitHub Pages unterscheidet Gross- und Kleinschreibung, deshalb müssen Dateinamen exakt stimmen, z. B. `assets/logo-full.png` und nicht `Assets/Logo-Full.png`.

## Projektstruktur

```text
HabitHero_LiveServer_v2/
├── index.html        # Struktur der Web-App
├── style.css         # Layout, Farben, Responsive Design
├── app.js            # Logik, Speicherung, Statistik, Gamification
├── manifest.json     # Basisinformationen für Web-App/PWA
├── README.md         # Kurzbeschreibung und Startanleitung
└── assets/
    ├── favicon.png
    ├── logo.png
    ├── logo-full.png
    └── logo-icon.png
```

## Start über GitHub Pages

1. Browser öffnen.
2. Folgende Adresse aufrufen: **https://haeusele83.github.io/habit_hero/**
3. Optional auf **Demo** klicken, damit sofort Beispiel-Habits, Statistikdaten und Badges sichtbar sind.
4. Die App kann anschliessend direkt getestet werden.

## Lokaler Start mit Visual Studio Code

1. Den Ordner `HabitHero_LiveServer_v2` in Visual Studio Code öffnen.
2. Falls noch nicht vorhanden: Die Erweiterung **Live Server** installieren.
3. Rechtsklick auf `index.html` machen.
4. **Open with Live Server** auswählen.
5. Die App öffnet sich automatisch im Browser.
6. Optional auf **Demo** klicken, damit sofort Beispiel-Habits, Statistikdaten und Badges sichtbar sind.

## Umgesetzte Hauptfunktionen

- Habits erfassen, bearbeiten und löschen
- Habits für den aktuellen Tag abhaken
- Tagesfortschritt mit Fortschrittsring anzeigen
- Suche und Filter für Habits
- XP- und Level-System
- Badges / Achievements als Gamification-Elemente
- Statistik mit Wochenübersicht, Heatmap und Habit-Erfolg
- JSON-Export und JSON-Import
- Demo-Daten für Präsentation und Test
- Responsives Layout für Desktop, Tablet und Smartphone

## Empfohlener Ablauf für die Live-Demo

1. App über GitHub Pages oder lokal mit Live Server öffnen.
2. Demo-Daten laden.
3. Dashboard zeigen: Tagesfortschritt, offene Habits und Level-Fortschritt.
4. Einen Habit abhaken und zeigen, wie sich Fortschritt und XP verändern.
5. Einen neuen Habit erfassen.
6. Statistik öffnen und Wochenübersicht, Heatmap sowie Habit-Erfolg erklären.
7. Badges anzeigen und Gamification kurz erläutern.
8. Optional JSON-Export zeigen, um die lokale Datensicherung zu demonstrieren.

## Abgrenzung

HabitHero ist ein MVP und keine produktive Cloud-Lösung. Die App arbeitet lokal im Browser und enthält bewusst keine Benutzerkonten, keine Synchronisation zwischen Geräten und keine Server-Datenbank. Diese Funktionen wären mögliche Erweiterungen für eine spätere Ausbaustufe.

## Hinweise zur Datenspeicherung

Alle Daten werden im jeweiligen Browser lokal gespeichert. Bei der Nutzung über GitHub Pages werden keine Daten an einen Server übertragen. Wird ein anderer Browser oder ein anderes Gerät verwendet, sind die lokal gespeicherten Habits dort nicht automatisch vorhanden. Für die Demonstration kann deshalb jederzeit die Funktion **Demo** genutzt werden.

## Kurzfazit

HabitHero erfüllt die zentralen Anforderungen des Projekts: Die App ist lauffähig, einfach testbar, visuell ansprechend und bildet die Kernfunktionen eines digitalen Habit-Trackers ab. Durch GitHub Pages ist die Anwendung ohne Installation erreichbar. Zusätzlich bleibt die technische Lösung mit HTML, CSS, JavaScript und Live Server schlank, nachvollziehbar und gut präsentierbar.
