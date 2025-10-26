# THC Legacy RP — A Tribute to Steve

**Release-Ziel:** 16.07.2028 • **Status:** In aktiver Entwicklung • **Plattform:** FiveM (GTA V)

## Warum dieses Projekt existiert

THC Legacy RP ist eine Liebeserklärung an die frühe Multiplayer-Ära und an Steve, dessen Begeisterung und Anspruch uns seit 2008 prägen. Wir bauen eine moderne Roleplay-Experience, die Technik, Wirtschaft und faires Miteinander vereint — mit derselben Liebe zum Detail, die damals den größten Server der Szene möglich machte.

## Vision in einem Satz

Eine lebendige, spielergetriebene Stadtökonomie mit echten Lieferketten, Behörden, Justiz und tiefer Fahrzeugsimulation — zugänglich, fair, langlebig und offen für Mitgestaltung.

## Leitprinzipien

* **Spielergetriebene Wirtschaft:** Produktion, Verarbeitung, Handel und Dienstleistungen greifen ineinander.
* **Governance & Rechtsstaat:** Gesundheitsamt, Zoll, Steuer, Gerichte und Anwälte sind aktives Gameplay.
* **Technische Sauberkeit:** Modular, serverseitig autoritativ, dokumentiert und erweiterbar.
* **Fairness & Respekt:** Klare Regeln, transparente Sanktionen, starke Anti-Abuse-Mechaniken.
* **Tribut an die Wurzeln:** Ideen aus MTA-Zeiten modern interpretiert.

## Kernpfeiler (Geplante Features)

### 1) Ökonomie & Lieferketten

* Einzelbetriebe wie Restaurants, Schnellimbisse, Hot-Dog-Stände und mehr.
* Großmarkt als Drehscheibe: Einkauf für Läden, Ankauf von Bauern und Fleischern.
* Farming & Butchery: Felder, Ernte, Schlachtung, Verarbeitung zu Chargen mit Qualität und Frische.
* Logistik: Kapazitäten, Kühlkette, Lieferaufträge, Schadens- und Qualitätsmodell.
* Import/Export am Hafen: Getränke und Exoten mit Zoll, Lizenzen und Schiffszyklen.

### 2) Behörden & Justiz (Governance-Layer)

* Gesundheitsamt: Inspektionen, Hygienepunkte, Verwarnungen, Bußgelder, temporäre Schließungen.
* Zoll: Container-Kanäle, Dokumentenprüfung, Abgaben, Beschlagnahme bei Falschangaben.
* Steuerbehörde: Umsatzsteuer-Journal, Quartalsmeldung, Prüfungen, Bescheide.
* Gerichte: Fälle, Beweise, Verhandlungen, Urteile mit automatisierten Folgen.
* Anwälte/Kanzleien: Zulassung, Mandate, Honorare, Akteneinsicht.

### 3) Fahrzeuge & Simulation

* Manuelle Schaltung mit Ganglimits, optionalem Motorschaden bei ausgeschaltetem Begrenzer.
* Werkstatt-Tuning: Begrenzer als kostenpflichtige Modifikation, wirtschaftlich eingebettet.

### 4) Community & RP-Erlebnis

* Transparente Regeln und durchsetzbare, eskalierende Maßnahmen.
* Events, Saisons, städtische Kampagnen (z. B. Sommerfest: höhere Nachfrage für bestimmte Waren).

---

## Erweiterungen für Creator & Community

### Streamer-Spotlight (Twitch)

Der Kanal **xdr_bobx** hostet das **THC Legacy RP Streamer-Spotlight**: kurze Talks, Highlight-Reels und Mini-Sessions mit Creator:innen aus der Stadt. Fokus auf **Kultur statt Clickbait** — mit klarer Anti-Toxik-Linie (Parasozial-/Beziehungsdramen → Permabann gemäß Chat-Regeln).

### Zukunftsmodul: "Legacy Motors" – Twitch Autohaus (P2W-frei)

**Optionales** Community-Feature: Zuschauer sammeln **Legacy‑Coins ✦** (Channel Points) im Stream und können **ausgewählte** Fahrzeuge **auch** damit einlösen. **Alle** Fahrzeuge bleiben **immer** regulär für **IC** kaufbar.

**Fairness-Garantie:** Kein LC↔IC-Tausch, keine exklusiven Vorteile, die es IC nicht gibt.

**Richtwert-Formel (experimentell):** LC ≈ `ceil(IC/25)`, auf nächste **50** aufrunden, **min. 100 LC**.
**Beispiele:** Roller **600 IC → 100 LC** (Minimum) • coquette3 **28.000 IC → 1.200 LC**.
**Limits (geplant):** max. **1 Fahrzeug / 14 Tage** pro Twitch-Account, Wertdeckel **30.000 IC / 30 Tage**, Verknüpfung **Twitch ↔ Discord ↔ Ingame-ID**.

> Status: Idee ist festgehalten und wird später gemeinsam umgesetzt, sobald die Kernsysteme stehen.

---

## Architektur (Kurzüberblick)

**Modulare Ressourcen mit klaren Schnittstellen.** Beispiele für geplante Module:

- **Ökonomie:** `thc-econ-core`, `thc-wholesale`, `thc-farming`, `thc-butchery`, `thc-import-export`, `thc-shops`, `thc-logistics`
- **Governance & Recht:** `thc-gov-core`, `thc-health` (Gesundheitsamt), `thc-customs` (Zoll), `thc-tax` (Steuer), `thc-court` (Gerichte), `thc-law` (Anwälte), `thc-prison`
- **Regelwerk & Onboarding:** `thc-rules-core` (Hardcore-RP-Regeln), `thc-beginner-district` (eigener Stadtteil zur Eingewöhnung), `thc-rules-nui` (ingame Lesbarkeit/Quiz)
- **LegacyOS (Operations & Self-Service):** `thc-legacyos` (Webpanel: RBAC, Tickets, Einsätze, Register), `thc-legacyos-academy`, `thc-legacyos-ledger`
- **Gameplay / QoL:** `thc-vehicles`, `thc-tuning`, `thc-admin-tools`, `thc-inspector`, `thc-telemetry`
- **Progression:** `thc-xp` (XP/Level für QBCore), `thc-driver-license` (Führerschein & Punkte, Caps/Entzug), `thc-perks`
- **Crime & Balance:** `thc-crime-core`, `thc-heists`, `thc-fencing` (Hehler), `thc-police-tools` (Beweise/Forensik)
- **Adapter & Safety:** Inventar-/Framework-Adapter für QBCore und/oder ox-ecosystem, serverseitige Validierung, Rate-Limits, Audit-Logs, Anti-Cheat-Hooks

---

## Roadmap (High Level)

- **2025 Q4 – 2026 H1:** Core-Design, Prototypen für Ökonomie & Gesundheitsamt, interne Tests; LegacyOS Grundgerüst (RBAC, Tickets).
- **2026 H2 – 2027 H1:** Großmarkt, Farming/Butchery-MVP, Shops mit Produktion & POS, erste Logistik-Loops; LegacyOS Register & Academy Alpha.
- **2027 H2:** Governance-Vertiefung (Zoll, Steuer, Court/Law), Balancing-Pässe; öffentliche Tech-Preview; XP/Level-Integration (`thc-xp`) als Opt-In.
- **2028 Q1:** Finalisierung **Hardcore-RP-Regeln** (`thc-rules-core`) & **Anfänger-Stadtteil** (`thc-beginner-district`), Führerschein/Punkte-Rework; LegacyOS Beta.
- **2028 H1:** Breite Content-Beta, Performance-Optimierung, Polishing, Dokumentation.
- **Release 16.07.2028:** **v1.0 – Stable**.

Ein detaillierteres, lebendes Board (Issues/Milestones) folgt im Repository.

## Mitmachen (Call for Contributors)

Wir suchen Menschen, die Lust haben, eine langlebige RP-Ökonomie zu bauen:

* Gameplay- und Systems-Designer:innen
* Lua-/JS-Entwickler:innen (FiveM, NUI)
* UI/UX, Technical Writers, Test & QA
* Community-Moderation und Event-Hosts

**Wie du startest:**

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
* Besonderer Dank an **Steve** und alle, die seit 2008 diese Reise möglich machen.

## Lizenz

Wird vor der ersten öffentlichen Beta festgelegt (Open-Source-orientiert). Vorschläge und Anforderungen gern als Issue diskutieren.

## Kontakt & Updates

* Discord: folgt
* Dev-Updates: Repo-Issues und Discussions

## Infrastruktur & Betrieb

**Aktueller Primär-Server:** AMD Ryzen™ 9 7950X3D (16C/32T), 128 GB ECC DDR5, 2× 1.92 TB NVMe, Standort: Falkenstein (DE)
---

**Kurzfassung:** THC Legacy RP vereint tiefe, faire Ökonomie mit echten Behörden- und Justizsystemen, moderner Fahrzeugtechnik und einer Community, die gemeinsam baut — als Tribut an die Anfänge und an Steve. Release-Ziel: 16.07.2028. Sei dabei.

Credit: Modernes XP-/Level-System für QBCore von RAzZ14 – https://github.com/RAzZ14
 – verwendet mit Dank & Respekt.
