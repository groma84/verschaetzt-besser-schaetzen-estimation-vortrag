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

- Einzelne Arbeitspakete für einen Sprint abschätzen
- Agile Schätzmethoden
- Riesenprojekte

---

# Definitionen

<img src="/images/definitionen-pisit-heng-FQvadXmA524-unsplash.jpg" class="w-120 object-fit-contain">

---

## Definitionen

<div v-click>

### Target/Ziel

Gewünschtes Geschäftsziel: "wir brauchen X, damit Y"

</div>

<div v-click>

### Commitment

Zusage: "Wir liefern X zum Zeitpunkt T in Qualität Q"

</div>

<div v-click>

### Estimate/Schätzung

Fragen: "Wie lange wird X dauern? Wie viel wird X kosten?"

</div>


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

<v-click>

- Aussagen wie "zu 90% sicher" machen nur Sinn, wenn es eine Faktenbasis gibt
- Sicherheit wird fast immer zu optimistisch angegeben (Realität: Leute denken 90%, sind aber eher 30% Treffsicherheit)
- Schätzung: je unsicherer, desto größer muss die Spannweite sein

</v-click>



---

## Wahrscheinlichkeiten und Gefahren

<v-clicks>

- Exakte Schätzung: "Es dauert 62 PT" 💣
- Erfolgschance von Projekten: Glockenkurve? 💣
- Es gibt eine untere Grenze, wie gut es laufen kann, **aber keine obere Grenze, wie schlecht**
- "Diseconomy of scale" 

</v-clicks>

<v-click>

<img src="/images/alles-kann-schlecht-werden-arash-payam-ww9DO6PsTBE-unsplash.jpg" class="mt-6 w-80 object-fit-contain">

</v-click>

---

## "Die Projektsteuerung rettet alles!"

<v-click>

- Projektsteuerung bringt Schätzung, Ziel und Commitment zusammen
- Gute Projektsteuerung kann bis zu 20% Fehler bei der Schätzung ausgleichen
- Je größer die Abweichungen, desto mehr Energie und Arbeit braucht die Steuerung

</v-click>


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

<v-click>

1) Unzureichende Informationen für die genaue Schätzung
2) Falsche Einschätzung der eigenen Fähigkeiten
3) Zuviel Veränderung im Projekt/in den Requirements
4) Schlechter Schätzprozess

</v-click>

---

## Unsicherheitstrichter

<img src="/images/unsicherheitstrichter.jpg" class="w-130 object-fit-contain" />



---

## Unsicherheitstrichter

<v-click>

- best-case!
- den Trichter schmaler bekommen ist kein Automatismus!
- Unsicherheitsfaktoren immer mitdenken
- **Spannungsfeld: Commitment (zu) früh im Trichter abgeben**

</v-click>

---

## Eigene Fähigkeiten

<v-click>

- Schätzung basiert z.B. auf "Seniors machen es"
- Umsetzung wird aber nicht nur von Seniors gemacht
- Abweichung zwischen Schätzung und echter Dauer  - muss nicht schlimm sein, muss aber berücksichtigt werden (Plan!, Abrechnung)

</v-click>

---

## Zuviel Veränderung

<v-click>

- Unklare Requirements
- Sich ändernde Requirements
- NASA plant immer 40% dafür extra ein

</v-click>

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

## Verfahren

- Zählen und Rechnen, Historische Daten
- Expertenschätzung, Gruppenreview
- Toolgestützt
- Formale Methoden

---

## Zählen und Rechnen

<v-clicks>

- man "zählt" etwas, das stark mit dem Aufwand korreliert (z.B. Anzahl an Formularen, Anzahl an anzubindenen Services, ...)
- man kennt den Aufwand pro Ding
- Gesamtaufwand: Anzahl * Aufwand
- Ideal: Es gibt mindestens 20 davon, damit sich eventuelle Fehler rausmitteln können

</v-clicks>

---

## Historische Daten

<v-clicks>

- Vorbedingung für Zählen und Rechnen: Man hat Daten aus der Vergangenheit
- Vorbedingung für nach und nach besser werdende Schätzungen: Man hat Daten aus der Vergangenheit
- Je besser man alte Daten erfasst hat (aus dem gleichen Projekt und aus ähnlichen Projekten), desto mehr Möglichkeiten hat man
- Regelmäßiger Abgleich Schätzung und echte Ergebnisse, um Fehler und Fehlerquellen zu finden

</v-clicks>

---

## Expertenschätzung

<v-click>

- "hinsetzen, nachdenken, abschätzen"
- "Umsetzungsexperte" vs. "Schätzexperte"
- Best case, worst case, most likely case
- Tipp: sich Zeit nehmen ("1% Regel"), nicht sofort auf Zuruf Einschätzung abgeben

</v-click>

---

## Expected case berechnen

- aus Best case, worst case, most likely case für spätere Rechnungen den Expected case pro Paket berechnen:

<div class="mt-5">
  <pre><code>Expected Case = (Best Case + (3 * Most Likely Case) + (2 * Worst Case)) / 6</code></pre>
</div>

---

## Bottom-up

<v-click>

- je feiner die Aufgliederung in Einzelpakete ist, desto weniger wird vergessen
- Checklisten benutzen
- je früher im Unsicherheitstrichter, desto gröber sind die Pakete. Das muss sich auch in der Schätzung widerspiegeln

</v-click>

---

## Mathematische Tücken

<v-click>

- einfach nur die Best Case und Worst Case Werte addieren klappt nicht!
- Stattdessen ein bisschen Mathe:
- $StdDev_{p} = \frac{(WorstCase_{p} - BestCase_{p})}{TeilerJeNachVertrauen}$
- Danach: $Varianz_{p} = StdDev_{p}^2$
- Am Ende: $StdDev = \sqrt{\sum{Varianz_{p}}}$

</v-click>

---

## Teiler je nach Vertrauen

<table style="line-height: 0.8rem; font-size: 0.8rem;">
  <tbody>
    <tr>
      <th>"% wirklich in 
      geschätzter Spannbreite"
      </th>
      <th>
      Teiler in Standardabweichung
      </th>
    </tr>
    <tr>
      <td>10</td><td>0,25</td>
    </tr>
    <tr>
      <td>20</td><td>0,51</td>
    </tr>
    <tr>
      <td>30</td><td>0,77</td>
    </tr>
    <tr>
      <td>40</td><td>1,00</td>
    </tr>
    <tr>
      <td>50</td><td>1,40</td>
    </tr>
    <tr>
      <td>60</td><td>1,70</td>
    </tr>
    <tr>
      <td>70</td><td>2,10</td>
    </tr>
    <tr>
      <td>80</td><td>2,60</td>
    </tr>
    <tr>
      <td>90</td><td>3,30</td>
    </tr>
    <tr>
      <td>99,7</td><td>6,00</td>
    </tr>
  </tbody>
</table> 


---

## Konfidenzintervalle

- Mit wieviel Wahrscheinlichkeit möchte ich unter dem Wert bleiben?
- Daraus bestimmt sich der Faktor für die Gesamt-Standardabweichung
- Die Einheiten müssen alle gleich sein (h, PT, Wochen, ...)

---

## Konfidenzintervalle

- $\sum{ExpectedCase} + (Faktor * StdDev)$

<table style="line-height: 0.8rem; font-size: 0.8rem;">
  <tbody>
    <tr>
      <th>Percentage confident</th>
      <th>Faktor
      </th>
    </tr>
    <tr>
      <td>10</td><td>-1,28</td>
    </tr>
    <tr>
      <td>20</td><td>-0,84</td>
    </tr>
    <tr>
      <td>30</td><td>-0,52</td>
    </tr>
    <tr>
      <td>40</td><td>-0,25</td>
    </tr>
    <tr>
      <td>50</td><td>0</td>
    </tr>
    <tr>
      <td>60</td><td>0,25</td>
    </tr>
    <tr>
      <td>70</td><td>0,52</td>
    </tr>
    <tr>
      <td>80</td><td>0,84</td>
    </tr>
    <tr>
      <td>90</td><td>1,28</td>
    </tr>
    <tr>
      <td>98</td><td>2</td>
    </tr>
  </tbody>
</table> 

---

## Geschafft

<img src="/images/mathe-geschafft-dan-cristian-padure-xJLN32FO7AY-unsplash.jpg" class="w-110 object-fit-contain" />

In der Praxis: Tools benutzen (z.B. ein Excel-Sheet)

---

## Review in der Gruppe

<v-click>

- Umsetzungsexperten UND Schätzexperten
- erst jeder für sich, dann austauschen und besprechen
- Formaler Prozess: [Wideband Delphi](https://en.wikipedia.org/wiki/Wideband_delphi)

</v-click>

---

## Wideband Delphi

0) Koordinator und Schätzexperten bestimmen
1) Koordinator verschickt die Spezifikation und ein Schätzformular
2) Meeting mit allen, um Unklarheiten in der Spezifikation zu besprechen
3) Jeder Experte füllt das Schätzformular **anonym** aus
4) Koordinator sammelt die Ergebnisse ein, führt sie zusammen und verteilt die Menge aller Schätzungen
5) Meeting mit allen, um extreme Abweichungen in den Schätzungen zu besprechen
6) Schritt 3-5 wiederholen, bis es keine extremen Abweichungen mehr gibt
7) Meeting mit allen, um die endgültige gemeinsame Abschätzung einstimmig anzunehmen


---

## Toolgestützt

- NDepend, JArchitect, ... für bestehende Software
- Simulation des Projektverlaufs
- Sanity Check von mit anderen Methoden erstellten Schätzungen
- Achtung: SHISHO ("Shit in, shit out")

---

## Formale Methoden

<div v-click> 

### COCOMO

- Constructive Cost Model
- Mathematische Formeln und viele (zuviele?) Rechenfaktoren
- Schwierig bei vielen Anforderungsänderungen

</div>

<div class="mt-7" v-click>

### Function Point Analyse

- ISO/IEC 20926
- Fokus auf fachlich-funktionale Anforderungen
- Achtung: Das Drumherum nicht vergessen

</div>

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

<div v-click>

### Wertung

<ul style="font-size: 0.8rem;">
  <li>10+ -> super</li>
  <li>7-9 -> tauglich für die Projektsteuerung, wahrscheinlich zu optimistisch geschätzt</li>
  <li>0-6 -> in der Praxis nutzlos</li>
</ul>

</div>

<p style="font-size: 0.7rem; margin-top: 0; font-style: italic;">The original "Estimate Sanity Check" is from Software Estimation by Steve McConnell (Microsoft Press, 2006) and is copyrighted in 2006 by Steve McConnell. All Rights Reserved. Permission to copy this quiz is granted provided that this copyright notice is included.</p>


---

## Kommunikation

<v-click>

- keine falsche Präzision!
- Je unsicherer, desto größer muss die Bandbreite sein
- Abgleich mit dem Plan
- die unwahrscheinlichen Fälle weglassen

</v-click>

---

## Bücher

<div style="display: flex;">
  <img src="/images/estimation-book-cover.jpg" class="w-80 object-fit-contain" />
  <img src="/images/optimales-projektmanagement-cover.jpg" class="w-70 ml-7 object-fit-contain" />
</div>

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

