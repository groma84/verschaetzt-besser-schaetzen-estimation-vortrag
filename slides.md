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

### Warum wir beim Schätzen meistens daneben liegen und wie es besser geht

##### Martin Grotz, MATHEMA GmbH

---

## Buch

<img src="/images/estimation-book-cover.jpg" class="w-80 object-fit-contain" />

---

## Agenda

---

## Definitionen

### Target/Ziel

Gewünschtes Geschäftsziel: "wir brauchen X um Y, **damit Z**"


### Commitment

Zusage: Wir liefern X zu Y in Qualität Q


### Estimate/Schätzung

Wie lange wird X dauern? Wie viel wird X kosten?


---

## Schätzung vs. Plan

<div v-click>

### Schätzung

- vorurteilsfrei
- faktenbasiert
- analytisch

</div>

<div v-click>

### Plan

- ergebnisoptimiert
- was wollen wir erreichen
- wie wollen wir es erreichen

</div>

---

## Wahrscheinlichkeiten und Gefahren

<v-clicks>

- Exakte Schätzung: "Es dauert 60 PT" 💣
- Glockenkurve 💣
- Es gibt eine untere Grenze, wie gut es laufen kann, aber keine obere Grenze, wie schlecht😲

</v-clicks>


---

## "Projektsteuerung rettet alles!"

<v-clicks>

- bringt Schätzung, Ziel und Commitment zusammen
- Gute Projektsteuerung kann bis zu 20% Fehler bei der Schätzung ausgleichen
- Je größer die Abweichungen, desto mehr Energie und Arbeit braucht die Steuerung

</v-clicks>

---

## Das Ziel der Schätzung

<v-clicks>

- Herausfinden, ob Ziel und Aufwand nah genug beieinander liegen, um mit Hilfe der Projektsteuerung realistisch verknüpft werden zu können 
- Dem Projektmanager eine solide Basis für Entscheidungen liefern

</v-clicks>

---

## Wie sicher bist du dir?

<v-clicks>

- Aussagen wie "zu 90% sicher" machen nur Sinn, wenn es eine Faktenbasis gibt
- Sicherheit wird fast immer zu optimistisch angegeben (Realität: Leute denken 90%, sind aber eher 30% Treffsicherheit)
- je unsicherer, desto größer muss die Spannweite sein

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

- Praktisch alle Schätzungen sind zu klein!
- Durchschnittliche echte Projektdauer: Schätzung +120%
- Durchschnittliche echte Projektkosten: Schätzung +100%

</div>

---

## Nutzen

Gute Schätzungen bringen:
- Echte Statusinformation
- Höhere Qualität
- Einfachere Kommunikation
- Planungssicherheit (Kunde und wir!)
- Vertrauen
- Erkannte Abweichungen liefern konkreten Anlass zur Risikobewertung

---

## Fehlerquellen

<v-clicks>

1) Unzureichende Informationen für die Schätzung
2) Falsche Einschätzung der eigenen Fähigkeiten
3) Zuviel Veränderung im Projekt/in den Requirements
4) Schlechter Schätzprozess

</v-clicks>

---

## Unzureichende Informationen

Unsicherheitstrichter

<img src="/images/cone-of-uncertainty-slide8-3016743625.png" class="w-110 object-fit-contain" />



---

## Unsicherheitstrichter

<v-clicks>

- best-case!
- den Trichter schmaler bekommen ist kein Automatismus!
- Unsicherheitsfaktoren immer mitdenken
- ggf. aufteilen: Person A schätzt "worst-case und best-case", Person B "wie unsicher ist es jeweils"
- **Problem: Commitment zu früh im Trichter abgegeben**

</v-clicks>

---

## Eigene Fähigkeiten

- Schätzung basiert auf "Seniors machen es"
- Umsetzung wird nicht (nur) von Seniors gemacht
- Abweichung zwischen Schätzung und echter Dauer  - muss nicht schlimm sein, muss aber berücksichtigt werden (Plan!)

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
  - ...

</div>

<div v-click>

Zahlen aus dem Buch: ca. 30% der Aufgaben (und damit Aufwände) werden von Entwicklern routinemäßig bei der Schätzung vergessen

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

## Meine eigenen Erfahrungen

- Uni Bamberg (abgeschlossen)
- Leistritz (läuft noch)
- CTI Systems Angular PoC (abgeschlossen)
- CTI Systems Code-Optimierung (noch nicht gestartet)

---

## Wie geht es besser?

<img src="/images/to-be-continued-unsplash.jpg" class="w-130 object-fit-contain" />


