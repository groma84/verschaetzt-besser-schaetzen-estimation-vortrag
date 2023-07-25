---
theme: ./mathema-2023

defaults:
  layout: "default-with-footer"

# infos for the footer (on slides with the default-with-footer layout)
occasion: "DWX Developer Week 2023"
occasionLogoUrl: "images/DWX_LogoIcon_2023-scaled.jpg.jpg"
company: "MATHEMA GmbH"
presenter: "Martin Grotz"
contact: "martin.grotz@mathema.de"

# apply any windi css classes to the current slide
class: 'text-center'

highlighter: shiki

lineNumbers: true

info: |
  ## Flow Design und Funktionale Programmierung


# page transition
transition: slide-left

# use UnoCSS
css: unocss

layout: cover
---

# Flow Design und Funktionale Programmierung

##### Martin Grotz, MATHEMA GmbH

---

## Flow Design: Beispiel

<!--
<img src="/images/withdraw-money-verfeinerung-1.png" class="w-160 object-fit-contain" />
-->

<img src="/images/withdraw-money-verfeinerung-1.svg" class="w-160 object-fit-contain" />


---

## Entwurf, Architektur, Design

<v-clicks>

- 🧠 Entwurf: Lösung der funktionalen Anforderungen
- 📐 Architektur: Lösung der nicht-funktionalen Anforderungen
- 🏛️ Design: Architektur & Entwurf

</v-clicks>

---

## Implementation und Entwurf

<v-clicks>

- 🛠️ die Implementation spiegelt den Entwurf wider
- ✋ Abweichungen sind zu vermeiden

</v-clicks>

---

## Vermischung

<v-click>

<img src="/images/vermischung-e-i.png" class="w-50 object-fit-contain" />

</v-click>

<v-click>

<img src="/images/blocks-e-i.png" class="w-50 object-fit-contain mt-8" />

</v-click>


<!--
  Auch bei TDD haben wir diese Vermischung: sogar noch mit Test dazwischen
-->

---

## Lohnt sich ein separater Entwurf überhaupt?

<v-click>

- "Ich arbeite doch eh nur alleine"
- "Das Programm ist so klein"
- "Entwurf ist kompliziert und kostet Zeit"

</v-click>

---

# Teil 1: Flow Design

<img src="/images/tweet-decomposition.png" class="w-60 object-fit-contain" />


---

## Flow Design

<v-click>

- entwickelt von Ralf Westphal und Stefan Lieser
- Methodik für den (gemeinsamen) Entwurf

</v-click>

<v-click>

- Ziele: 
  - Nachdenken vor dem Umsetzen!
  - Probleme in kleinere Bausteine zerlegen

</v-click>

---

## Quellen

[https://flow-design.info/](https://flow-design.info/)

Buch: 
<img src="/images/flow-design-buch-cover.jpg" class="w-50 object-fit-contain" />

---

## Wofür nutze ich es?

<v-clicks>

- Zerlegung beibringen in der Lehre 
- Entwurf einer Lösung vor dem konkreten Lösen einer Aufgabenstellung
- Ideenweitergabe im Projekt
- Diskussion eines Entwurfs in der Gruppe

</v-clicks>



---

## Hilfsmittel

<v-click>

- analog: Stift&Papier, Whiteboard
- digital: excalidraw, Miro, ...

</v-click>

<v-click>

- beides hat Vor- und Nachteile
- [Cheatsheet von flow-design.info](https://flow-design.info/wp-content/uploads/2021/12/CheatSheet-Clean-Code-Developer-Akademie.pdf)

</v-click>

<!--
Küste Norwegens Problem -> digital leichter editierbar, am Ende Screenshot und ans Ticket ran
-->

---

## Flow Design: Vorgehensweise

1) System-Umwelt-Diagramm
2) Interaktionen
3) Entwurf der obersten Ebene
4) Verfeinerung

---

## Interaktionen und Oberste Ebene

<img src="/images/banking-interaktionen-1.svg" class="w-110 object-fit-contain" />

---

## Erste Verfeinerung: Withdraw Money

<img src="/images/withdraw-money-verfeinerung-1.svg" class="w-150 object-fit-contain" />

<!--

Portal: Zuständig für Zugriff von Client auf System
Logik: Funktionseinheit mit Domänenlogik

Einfacher Datenfluss: unit, Tupel, Menge
Datentypen
Split
Join
Fallunterscheidung mit "Callbacks"

-->

---

## Weitere Verfeinerung: Is Session Valid

<img src="/images/withdraw-verfeinerung-session-valid-1.svg" class="w-170 object-fit-contain" />

<!--
Provider
Ressourcen
Exceptions
-->


---

## Verfeinerung: Show Balance

<img src="/images/show-balance-verfeinerung-2.svg" class="w-200 object-fit-contain" />

<!--
"Mehrfachanwendung"/Schleifen
Verfeinerung von Verfeinerung
-->


---

## Composition Root

<v-clicks>

- konfiguriert die Komponenten und Abhängigkeiten
- möglichst nahe am Einstiegspunkt
- Beispiele: 
  - main-Methode in einer Konsolenanwendung
  - Controller in einem Web-Backend
  - Setup in ASP.NET Core

</v-clicks>

---

## Ressourcen "infizieren" die Logik

<img src="/images/abhaengigkeiten-ohne-interactor-quer.svg" class="w-150 object-fit-contain" />

---

## Pure Logik durch Interactor/Workflows

<img src="/images/abhaengigkeiten-mit-interactor-quer.svg" class="w-100 object-fit-contain" />


---

# Teil 2: Funktionale Programmierung

---

## Grundlagen der Funktionalen Programmierung

<v-clicks>

- Funktionen als Parameter und Rückgabewerte
- Daten ohne Logik
- Transformationen auf diesen Daten
- Kleine Funktionen zu größeren Funktionseinheiten komponieren
- Immutability
  
</v-clicks>

---
layout: two-images
---

## Flows

:: left ::

<v-click>

<img src="/images/calculate-balance-fuer-fp-1.png" class="w-100 object-fit-contain" />

</v-click>

:: right ::

<v-click>

<img src="/images/calculate-balance-verfeinerung-code-1.png" class="w-120 object-fit-contain" />

</v-click>

---
layout: two-images
---

## Flows

:: left ::

<v-click>

<img src="/images/get-balance-fuer-fp-1.png" class="w-100 object-fit-contain" />

</v-click>

:: right::

<v-click>

<img src="/images/get-balance-fuer-fp-code-1.png" class="w-120 object-fit-contain" />

</v-click>

---

## Fallunterscheidung / Union Types

<img src="/images/pattern-matching-entwurf-1.svg" class="w-140 object-fit-contain" />

<v-click>

<img src="/images/union-type-1.png" class="w-70 object-fit-contain" />

</v-click>

---
layout: two-images
---
## Fallunterscheidung: Return Type Problematik

:: left ::

<v-click>

<img src="/images/pattern-matching-ohne-functions.png" class="w-100 object-fit-contain" />

</v-click>

:: right ::

<v-click>

<img src="/images/pattern-matching-mit-functions-und-return-type.png" class="w-100 object-fit-contain" />

</v-click>

<!--
Ich muss ans Ende des Gesamtflows schauen, um rauszufinden, welchen Return Type ich für die einzelnen Fallunterscheidungsfunktionen angeben muss 
-->

---
layout: two-images
---
## Exkurs: Railway Oriented Programming

:: left ::

<v-click>

<div>

<img src="/images/railway-oriented-programming-entwurf-1.png" class="w-120 object-fit-contain" />

[Scott Wlaschin — Railway oriented programming](https://www.youtube.com/watch?v=fYo3LN9Vf_M)

</div>

</v-click>

:: right ::

<v-click>

<div>

<img src="/images/railway-oriented-programming-code-1.png" class="w-100 object-fit-contain" />

"Monadische Komposition"

</div>

</v-click>


---
layout: two-images
---
## Mein Fazit

:: left ::

<div style="font-size: 1rem;">

<v-click>


- **Was ich mag**:
  - fördert eine strukturierte Vorgehensweise
  - hilft in der Kommunikation
  - passt sehr gut zur Funktionalen Programmierung
    - Flows als Funktionen und Pipelines
    - Innerer Zustand nur als "notwendiges Übel"
    - Logik frei von Abhängigkeiten -> Pure Funktionen
  - resultiert in sauberer Architektur auf Komponentenebene
  - kommt mit relativ wenigen Elementen aus


</v-click>

<v-click>

- **Was ich nicht so mag**:
  - Fallunterscheidungen: Notation und Return Type
  - Schnelle Iterationen auf dem Entwurf sind aufwendig

</v-click>

</div>

:: right ::

<div>

<v-click>


<img src="/images/go-with-the-flow.jpg" class="w-60 object-fit-contain" />

Go with the flow (design)!


</v-click>

</div>


---

## Weitere spannende Vorträge

<img src="/images/von-csharp-zu-fsharp-vortragswerbung.png" class="w-120 object-fit-contain" />

<img src="/images/funktionales-csharp-vortragswerbung.png" class="w-120 object-fit-contain" />


---

## Kontakt

<div class="flex">
  <img alt="Martin Grotz Gesicht auf Briefkasten" src="images/martin_auf_briefkasten.jpg"  class="w-60 object-fit-contain"/>

  <table class="ml-4">
  <tbody>
    <tr>
      <td>E-Mail</td>
      <td><a href="mailto:martin.grotz@mathema.de">martin.grotz@mathema.de</a></td>
    </tr>
    <tr>
      <td>Twitter</td>
      <td><a href="https://twitter.com/mobilgroma">@mobilgroma</a></td>
    </tr>
    <tr>
      <td>Github</td>
      <td><a href="https://github.com/groma84/">groma84</a></td>
    </tr>
    
  </tbody>
  </table>
</div>


