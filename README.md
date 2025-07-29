# Øvingsoppgave - Pseudo-elementer/selektorer

Dette prosjektet er laget for å øve på bruk av pseudo-elementer (`::before`, `::after`) og pseudo-selektorer (`:hover`, `:first-child`, `:nth-child`, `:not()` osv.) i CSS. 

Målet er å gi HTML-elementer mer avansert og interaktiv styling uten å endre selve HTML-strukturen.

---

## 📁 Mappestruktur

```
pseudo-oppgave/
├── index.html      # HTML-strukturen
├── style.css       # All styling med pseudo-elementer og -selektorer
└── README.md       # Forklaringer på løsningen
```

---

## 🔧 Teknologier brukt

- HTML5
- CSS3 (fokus på pseudo-elementer og pseudo-selektorer)

---

## 🧩 Innhold og funksjoner

### ✅ HTML-struktur

- `<h1>` hovedoverskrift: "Lær Pseudo-elementer"
- `<ul>` uordnet liste med 5 elementer
- `<section>` med 3 `<div>` underseksjoner
- `<button>` med hover-effekt
- En ekstra seksjon med input-felt (`<div class="highlight">`)

---

## 🎨 CSS-forklaring

### Del 1: Pseudo-elementer

- `h1::before`  
  Lager en dekorativ linje til venstre for overskriften.

- `ul li::after`  
  Legger til en stjerne (`★`) etter hvert listeelement.

- Farge og størrelse:  
  Linjen (`::before`) har blå farge og fast bredde. Stjernen (`::after`) er gyllen og litt større enn vanlig tekst.

---

### Del 2: Pseudo-selektorer

- `li:nth-child(odd)`  
  Gir annen bakgrunn til annethvert listeelement (oddetall).

- `li:first-child`, `li:last-child`  
  Spesielle tekstfarger til det første (grønn) og siste (mørkerød) elementet.

- `li:not(:nth-child(3))`  
  Alle unntatt det tredje listeelementet får kursiv tekst.

- `button:hover`  
  Når du holder musen over knappen, endres bakgrunnsfargen med en jevn overgang (`transition`).

---

### Ekstra utfordring

- `.highlight::before` og `::after`  
  Lager en dobbel dekorativ ramme rundt teksten i en seksjon.

- `input:focus`  
  Når input-feltet er i fokus, får det tydelig oransje kant og lys bakgrunn.

- `section div:nth-of-type(2)`  
  Fremhever andre underseksjon med grønn bakgrunn og fet skrift.

---

## ▶️ Bruk

1. Åpne `index.html` i en nettleser.
2. Inspiser elementene og hover over knappen.
3. Klikk i input-feltet og se effektene.
4. Endre CSS-filen for å teste egne ideer.

---

## 🧠 Hva du lærer

- Hvordan bruke pseudo-elementer til dekorativt innhold.
- Hvordan bruke pseudo-selektorer for å målrette styling basert på struktur.
- Hvordan gjøre siden mer dynamisk og brukervennlig uten JavaScript.
