---
theme: ./mathema-2023

defaults:
  layout: "default-with-footer"

# infos for the footer (on slides with the default-with-footer layout)
occasion: "enterJS 2024"
occasionLogoUrl: "images/enterjs.svg"
company: "MATHEMA GmbH"
presenter: "Martin Grotz"
contact: "martin.grotz@mathema.de"

# apply any windi css classes to the current slide
class: 'text-center'

highlighter: shiki

lineNumbers: true

info: |
  ## Verschätzt - Warum wir beim Schätzen meistens daneben liegen und wie es besser geht


# page transition
transition: slide-left

# use UnoCSS
css: unocss

layout: cover
---

# Verschätzt! 

### Warum wir beim Schätzen meistens daneben liegen... 

### und wie es besser geht

##### Martin Grotz, MATHEMA GmbH



---

## Agenda

- Definitionen
- Probleme
- Lösungen

---

# Über was reden wir nicht

- Einzelne Arbeitspakete abschätzen
- Agile Schätzmethoden
- Riesenprojekte

---

# Definitionen

<img src="/images/definitionen-pisit-heng-FQvadXmA524-unsplash.jpg" class="w-120 object-fit-contain">

---

## Definitionen

### Target/Ziel

Gewünschtes Geschäftsziel: "wir brauchen X, damit Y"


### Commitment

Zusage: "Wir liefern X zum Zeitpunkt T in Qualität Q"


### Estimate/Schätzung

Fragen: "Wie lange wird X dauern? Wie viel wird X kosten?"


---

## Schätzung vs. Plan

<div v-click>

### Schätzung

- vorurteilsfrei
- faktenbasiert
- analytisch

</div>

<div class="mt-7" v-click>

### Plan

- ergebnisoptimiert
- was wollen wir erreichen
- wie wollen wir es erreichen

</div>

---

## Nutzen einer guten Schätzung

<v-click>

Gute Schätzungen bringen:
- Echte Statusinformation
- Höhere Qualität
- Einfachere Kommunikation
- Planungssicherheit (Kunde und wir!)
- Vertrauen
- Erkannte Abweichungen liefern konkreten Anlass zur Risikobewertung

</v-click>


---

# Probleme

<img src="/images/probleme-kelly-sikkema-CbZC2KVnK8s-unsplash.jpg" class="w-120 object-fit-contain">


---

## Das Ziel der Schätzung

<v-clicks>

- "Herausfinden, ob Ziel, Plan und Aufwand nah genug beieinander liegen, um mit Hilfe der Projektsteuerung realistisch verknüpft werden zu können"
- Dem Projektmanager eine solide Basis für Entscheidungen liefern

</v-clicks>

---

## Wie sicher bist du dir?

<v-clicks>

- Aussagen wie "zu 90% sicher" machen nur Sinn, wenn es eine Faktenbasis gibt
- Sicherheit wird fast immer zu optimistisch angegeben (Realität: Leute denken 90%, sind aber eher 30% Treffsicherheit)
- Schätzung: je unsicherer, desto größer muss die Spannweite sein

</v-clicks>



---

## Wahrscheinlichkeiten und Gefahren

<v-clicks>

- Exakte Schätzung: "Es dauert 62 PT" 💣
- Erfolgschance von Projekten: Glockenkurve? 💣
- Es gibt eine untere Grenze, wie gut es laufen kann, **aber keine obere Grenze, wie schlecht**
- "Diseconomy of scale" 

<img src="/images/alles-kann-schlecht-werden-arash-payam-ww9DO6PsTBE-unsplash.jpg" class="mt-6 w-80 object-fit-contain">

</v-clicks>

---

## "Die Projektsteuerung rettet alles!"

<v-clicks>

- Projektsteuerung bringt Schätzung, Ziel und Commitment zusammen
- Gute Projektsteuerung kann bis zu 20% Fehler bei der Schätzung ausgleichen
- Je größer die Abweichungen, desto mehr Energie und Arbeit braucht die Steuerung

</v-clicks>


---

## Zuviel oder zuwenig

<div v-click>

- zu groß schätzen?
  - Parkinson's Law (Arbeit füllt immer die zur Verfügung stehende Zeit)
  - "Gold-plating" Gefahr

</div>

<div v-click>

- zu klein schätzen?
  - Projektpläne sind wertlos
  - Steuerungsaufwand steigt (Krisenmeetings, Kommunikation mit dem Kunden, ...)
  - Qualität sinkt
  - Entwickler schätzen eh schon immer zu optimistisch

</div>

---

## Systemisches Problem

<div v-click>

- Praktisch alle Schätzungen sind zu <span style="font-size: 1rem;">klein</span>!
- Durchschnittliche echte Projekt**dauer**: Schätzung <span style="color: red; font-weight: bold;">+120%</span>
- Durchschnittliche echte Projekt**kosten**: Schätzung <span  style="color: red; font-weight: bold;">+100%</span>

</div>

---

## Fehlerquellen

<v-clicks>

1) Unzureichende Informationen für die Schätzung
2) Falsche Einschätzung der eigenen Fähigkeiten
3) Zuviel Veränderung im Projekt/in den Requirements
4) Schlechter Schätzprozess

</v-clicks>

---

## Unsicherheitstrichter

<img src="/images/unsicherheitstrichter.jpg" class="w-130 object-fit-contain" />



---

## Unsicherheitstrichter

<v-clicks>

- best-case!
- den Trichter schmaler bekommen ist kein Automatismus!
- Unsicherheitsfaktoren immer mitdenken
- **Spannungsfeld: Commitment (zu) früh im Trichter abgeben**

</v-clicks>

---

## Eigene Fähigkeiten

- Schätzung basiert z.B. auf "Seniors machen es"
- Umsetzung wird aber nicht nur von Seniors gemacht
- Abweichung zwischen Schätzung und echter Dauer  - muss nicht schlimm sein, muss aber berücksichtigt werden (Plan!, Abrechnung)

---

## Zuviel Veränderung

- Unklare Requirements
- Sich ändernde Requirements
- NASA plant immer 40% dafür extra ein

---

## Wir haben da was vergessen... Schätzung

Nebenaufgaben werden oft vergessen:

<div v-click>

  - Setup bei jedem Entwickler
  - Testdaten generieren
  - Setup CI/CD
  - Deployment auf dem Endsystem
  - Onboarding
  - Kommunikation mit dem Kunden
  - Regelmäßige Meetings
  - Änderungen nach Reviews
  - ...

</div>

---

## Wir haben da was vergessen... Plan

Manche Dinge erhöhen den Aufwand nicht, aber die Projektdauer schon:

<div v-click>

  - Urlaub
  - Krankheit
  - Fortbildung
  - Hardware-Probleme
  - ...

</div>


---

## Schlechter Schätzprozess

<div v-click>

- Unbegründeter Optimismus
- Druck von außen
- Zuviele Stellschrauben bei den Schätz-Faktoren   
- Zu hohe (angebliche) Präzision
- Zu schnell abgeschätzt

</div>

---

# Lösungen

<img src="/images/loesungen-riccardo-annandale-7e2pe9wjL9M-unsplash.jpg" class="w-120 object-fit-contain" />

---

Verfahren
- Zählen und Rechnen, Historische Daten
- Expertenschätzung, Gruppenreview
- Zerlegen und Zusammensetzen
- Analogien und Proxys
- Toolgestützt
- Formale Methoden

---

## Zählen und Rechnen

---

## Historische Daten

---

## Expertenschätzung

---

## Review in der Gruppe

---

## Zerlegen und Zusammensetzen

---

## Analogien und Proxys

---

## Toolgestützt

- NDepend, JArchitect, ... für bestehende Software
- Simulation des Projektverlaufs
- Sanity Check von mit anderen Methoden erstellten Schätzungen
- Achtung: SHISHO ("Shit in, shit out")

---

## Formale Methoden

### COCOMO

- Constructive Cost Model
- Mathematische Formeln und viele (zuviele?) Rechenfaktoren
- Schwierig bei vielen Anforderungsänderungen

### Function Point Analyse

- ISO/IEC 20926
- Fokus auf fachlich-funktionale Anforderungen
- Achtung: Das Drumherum nicht vergessen

---

# Estimate Sanity Check

<div style="display: flex;" class="mb-5">
    <ul style="font-size: 0.8rem;">
      <li>Wurde ein definierter Prozess zur Erstellung genutzt?</li>
      <li>War die Erstellung frei von externem Druck/externer Einflussnahme?</li>
      <li>Wenn Sachen verhandelt wurde, ging es nur um Eingabedaten für die Schätzung?</li>
      <li>Entspricht die Präzision der Angabe der Projektphase? (Unsicherheitstrichter)</li>
      <li>Wurden unterschiedliche Schätztechniken eingesetzt, die zu ähnlichen Ergebnissen kamen?</li>
      <li>Ist die angenommene Produktivität der Projektbeteiligten aus der Vergangenheit begründbar?</li>
    </ul>
    <ul style="font-size: 0.8rem;">
      <li>Ist die Dauer des Plans mindestens 2x der Aufwand?</li>
      <li>Waren die Leute, die später an der Umsetzung beteiligt sind, auch an der Schätzung beteiligt?</li>
      <li>Wurde die Schätzung nochmal von mindestens einem Experten geprüft?</li>
      <li>Enthält die Schätzung einen Puffer für Projektrisiken?</li>
      <li>Gehört die Schätzung zu einer Reihe von immer genaueren Schätzungen im Projektverlauf?</li>
      <li>Wurde an alle Aufgaben innerhalb des Projekts und innerhalb jedes Arbeitspakets gedacht?</li>
    </ul>

</div>

### Wertung

<ul  style="font-size: 0.8rem;">
<li>10+ -> super</li>
<li>7-9 -> tauglich für die Projektsteuerung, wahrscheinlich zu optimistisch geschätzt</li>
<li>0-6 -> in der Praxis nutzlos</li>
</ul>

<p  style="font-size: 0.7rem; margin-top: 0; font-style: italic;">The original "Estimate Sanity Check" is from Software Estimation by Steve McConnell (Microsoft Press, 2006) and is copyrighted in 2006 by Steve McConnell. All Rights Reserved. Permission to copy this quiz is granted provided that this copyright notice is included.</p>


---

## Buch

<img src="/images/estimation-book-cover.jpg" class="w-80 object-fit-contain" />

---

## Kontakt

<div class="flex">
  <img alt="Martin Grotz Gesicht auf Briefkasten" src="/images/martin_auf_briefkasten.jpg"  class="w-60 object-fit-contain"/>

  <table class="ml-4">
  <tbody>
    <tr>
      <td>E-Mail</td>
      <td><a href="mailto:martin.grotz@mathema.de">martin.grotz@mathema.de</a></td>
    </tr>
     <tr>
      <td>LinkedIn</td>
      <td><a href="https://www.linkedin.com/in/martin-grotz-6780332b5/">https://www.linkedin.com/in/martin-grotz-6780332b5/</a></td>
    </tr>
    <tr>
      <td>MATHEMA Github</td>
      <td><a href="https://github.com/MATHEMA-GmbH/">MATHEMA-GmbH</a></td>
    </tr>
    <tr>
      <td>Privates Github</td>
      <td><a href="https://github.com/groma84/">groma84</a></td>
    </tr>
  </tbody>
  </table>
</div>

