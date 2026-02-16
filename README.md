# THC Legacy RP — A Tribute to Steve

**Release-Ziel:** 16.07.2028 • **Status:** In aktiver Entwicklung • **Plattform:** MTA (GTA SA)

## Warum dieses Projekt existiert

THC Legacy RP ist eine Liebeserklärung an die frühe Multiplayer-Ära und an Steve, dessen Begeisterung und Anspruch uns seit 2008 prägen. Wir bauen eine moderne Roleplay-Experience auf MTA, die Technik, Wirtschaft und faires Miteinander vereint — mit derselben Liebe zum Detail, die damals den größten Server der Szene möglich machte.

## THC Legacy – Historische Basis (2008–2017)

Wir haben unsere alten THC-Dateien aus der MTA-Ära wiederentdeckt. Sie dienen heute als **kreative Vorlage**: Spielmechaniken, Balancing-Ideen, Anticheat-Ansätze und UI-Konzepte. Alles wird **sauber für MTA neu gedacht und umgesetzt** – technisch modern, performancetauglich und modular.

Eine lebendige, spielergetriebene Stadtökonomie mit echten Lieferketten, Behörden, Justiz und tiefer Fahrzeugsimulation — zugänglich, fair, langlebig und offen für Mitgestaltung.

* **No Pay-2-Win:** Keine spielentscheidenden Vorteile gegen Geld; Progression & Balance bleiben fair.
  (Geplante Features)

### 1) Ökonomie & Lieferketten

* Einzelbetriebe wie Restaurants, Schnellimbisse, Verkaufsstände und mehr.
* Großmarkt als Drehscheibe: Einkauf für Läden, Ankauf von Produzenten.
* Farming & Verarbeitung: Felder, Ernte, Verarbeitung zu Chargen mit Qualität und Frische.
* Logistik: Kapazitäten, Lieferaufträge, Schadens- und Qualitätsmodell.
* Hafen- & Importmechaniken: Waren mit Lizenzen, Kontrollen und Zyklen.

### 2) Behörden & Justiz (Governance-Layer)

* Gesundheitsamt: Inspektionen, Hygienepunkte, Verwarnungen, Bußgelder, temporäre Schließungen.
* Kontroll-/Zollmechaniken: Dokumentenprüfung, Abgaben, Beschlagnahme bei Verstößen.
* Steuerbehörde: Umsatzjournal, Meldungen, Prüfungen, Bescheide.
* Gerichte: Fälle, Beweise, Verhandlungen, Urteile mit automatisierten Folgen.
* Anwälte/Kanzleien: Zulassung, Mandate, Honorare, Akteneinsicht.

### 3) Fahrzeuge & Simulation

* Manuelle Schaltung mit Ganglimits, optionalem Motorschaden bei ausgeschaltetem Begrenzer. **Original von 2009**
* Werkstatt-Tuning: Begrenzer als kostenpflichtige Modifikation, wirtschaftlich eingebettet.

### 4) Community & RP-Erlebnis

* Transparente Regeln und durchsetzbare, eskalierende Maßnahmen.
* Events, Saisons, städtische Kampagnen (z. B. Sommerfest: höhere Nachfrage für bestimmte Waren).

## Welt & Karte

* **Standardkarte (San Andreas):** bewusst gewählt für **Performance, Zugänglichkeit und Kompatibilität**.
* **THC-Feeling Map:** Eigene Zonen, Events, Lieferketten, Routen und dezente strukturelle Ergänzungen.
* **Anfänger-Stadtteil:** Geschützter Bereich zum Einsteigen (Jobs, Regeln, Schulungen) – bleibt ein fester Bestandteil.

## Architektur (Kurzüberblick)

Modulare Ressourcen mit klaren Schnittstellen. Beispiele für geplante Module:

* Ökonomie: thc-econ-core, thc-wholesale, thc-farming, thc-production, thc-import, thc-shops, thc-logistics
* Governance: thc-gov-core, thc-health, thc-control, thc-tax, thc-court, thc-law
* Gameplay/Quality-of-Life: Fahrzeug- und Tuning-Module, Admin-/Inspektions-Tools

Serverseitige Validierung, Rate-Limits, Audit-Logs.

## Roadmap (High Level)

* **2025 Q4–2026 H1**: Core-Design, Prototypen für Ökonomie und Gesundheitsamt, interne Tests.
* **2026 H2–2027 H1**: Großmarkt, Produktions-MVP, Shops mit POS, erste Logistik-Schleife.
* **2027 H2**: Governance-Vertiefung (Kontrolle, Steuer, Court/Law), Balancing-Pässe, geschlossene Tech-Preview.
* **2028 H1**: Beta mit Content-Breadth, Performance-Optimierung, Polishing, Dokumentation.
* **Release 16.07.2028**: v1.0 – Stable.

Ein detaillierteres, lebendes Board (Issues/Milestones) folgt im Repository.

## Mitmachen (Call for Contributors)

Wir suchen Menschen, die Lust haben, eine langlebige RP-Ökonomie auf MTA zu bauen:

* Gameplay- und Systems-Designerinnen und -Designer
* Lua-Entwicklerinnen und -Entwickler (MTA)
* UI/UX, Technical Writers, Test & QA
* Community-Moderation und Event-Hosts

Wie du startest:

1. Repository beobachten und Diskussionen verfolgen.
2. Themen in Issues aufgreifen oder neue Vorschläge einreichen.
3. Kleine, fokussierte Aufgaben übernehmen; wir helfen beim Onboarding.

## Community & Verhalten

* Respekt, Inklusion, kein Tox-Verhalten.
* Keine Exploits, kein Real-Money-Trade.
* Moderation mit klaren, dokumentierten Eskalationsstufen.
  Ein formeller Verhaltenskodex wird im Repo verlinkt.

## Rechtliches & Credits

* Inoffizielles Fanprojekt; alle Marken und Inhalte gehören ihren jeweiligen Rechteinhabern.
* Kein kommerzieller Vertrieb des Basisspiels oder seiner Assets.
* Besonderer Dank an Steve und alle, die seit 2008 diese Reise möglich machen.

## Lizenz

Wird vor der ersten öffentlichen Beta festgelegt (Open-Source-orientiert). Vorschläge und Anforderungen gern als Issue diskutieren.

## Kontakt & Updates

* Discord: folgt
* Dev-Updates: Repo-Issues und Discussions

---

**Kurzfassung:** THC Legacy RP vereint tiefe, faire Ökonomie mit echten Behörden- und Justizsystemen, moderner Fahrzeugtechnik und einer Community, die gemeinsam baut — als Tribut an die Anfänge und an Steve. Release-Ziel: 16.07.2028. Sei dabei.
