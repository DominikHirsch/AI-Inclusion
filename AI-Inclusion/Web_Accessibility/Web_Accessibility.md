---
title: Web Accessibility
---

# Web Accessibility

**Web Accessibility** (Barrierefreiheit im Web) beschreibt die Praxis, Webseiten, Inhalte und digitale Anwendungen so zu gestalten, dass sie für alle Menschen zugänglich und nutzbar sind – unabhängig von körperlichen, sensorischen oder kognitiven Einschränkungen.

Barrierefreies Webdesign ist nicht nur ein ethisches und rechtliches Thema, sondern verbessert auch die Nutzerfreundlichkeit für alle Menschen, einschließlich älterer Nutzer*innen, Menschen mit temporären Einschränkungen oder Personen mit langsamer Internetverbindung.

---

## 1. Was ist Web Accessibility?

Web Accessibility bedeutet, dass Menschen mit Behinderungen:

- Webseiten **wahrnehmen** können (z. B. per Screenreader),
- mit Inhalten **interagieren** können (z. B. mit der Tastatur navigieren),
- und Inhalte **verstehen** können (klare Sprache, strukturierte Inhalte).

Die **W3C** definiert Barrierefreiheit über die „**POUR-Prinzipien**“:

| Prinzip  | Bedeutung                              |
|----------|----------------------------------------|
| **P**erceivable | Informationen müssen für alle wahrnehmbar sein. |
| **O**perable    | Bedienung muss auf verschiedenen Wegen möglich sein. |
| **U**nderstandable | Inhalte müssen verständlich sein. |
| **R**obust      | Inhalte müssen mit verschiedenen Technologien funktionieren. |

---

## 2. Warum ist Barrierefreiheit wichtig?

### ✅ Gesellschaftlich:
- Menschen mit Behinderungen haben das Recht auf gleichberechtigten Zugang zu Informationen.
- Digitale Teilhabe ist ein Menschenrecht (UN-Behindertenrechtskonvention, Art. 9).

### ✅ Wirtschaftlich:
- Barrierefreie Seiten erreichen mehr Menschen (z. B. ältere Nutzer*innen, mobile Nutzer).
- Suchmaschinen bevorzugen strukturierte, barrierearme Seiten (SEO-Vorteile).

### ✅ Rechtlich:
- In vielen Ländern sind barrierefreie Angebote gesetzlich verpflichtend (z. B. EU-Richtlinie 2016/2102, Barrierefreiheitsstärkungsgesetz in Deutschland ab 2025).

---

## 3. Häufige Problemfelder

### 🔴 3.1 Nicht zugängliche Navigation

- Keine Tastaturbedienung möglich
- Fokusreihenfolge unlogisch
- Keine „Skip to Content“-Links

### 🔴 3.2 Unzureichende semantische Struktur

- Verwendung von `<div>` statt echten Überschriften (`<h1>`, `<h2>`)
- Fehlende Landmarken (`<nav>`, `<main>`, `<footer>`)

### 🔴 3.3 Fehlende Alternativtexte

- Bilder ohne `alt`-Text sind für Screenreader-Nutzer unsichtbar
- `alt`-Texte sind nicht beschreibend genug

### 🔴 3.4 Farbkontraste und visuelle Gestaltung

- Texte mit zu wenig Kontrast (z. B. hellgrau auf weiß)
- Bedeutung wird ausschließlich über Farbe vermittelt (z. B. grün = OK, rot = Fehler)

### 🔴 3.5 Dynamische Inhalte ohne ARIA

- Interaktive Komponenten (Modals, Dropdowns, Tabs) sind nicht screenreader-kompatibel
- Fehlende ARIA-Rollen und -Attribute (`role="dialog"`, `aria-expanded`, etc.)

### 🔴 3.6 Captions & Transkripte fehlen

- Keine Untertitel für Videos
- Kein Transkript für Audioinhalte

---

## 4. Best Practices & Techniken

### ✅ Semantisches HTML nutzen

- Nutze `h1–h6` für Überschriften  
- Nutze Listen (`<ul>`, `<ol>`) korrekt  
- Setze `<label>`-Elemente bei Formularfeldern

### ✅ ARIA richtig einsetzen (nicht übertreiben!)

- Nur verwenden, wenn native HTML-Elemente nicht ausreichen
- Beispiele: `aria-label`, `aria-hidden`, `aria-describedby`

### ✅ Tastaturzugänglichkeit sicherstellen

- Alle Funktionen per `Tab`-Taste erreichbar machen
- Sichtbaren Fokus für aktive Elemente anzeigen

### ✅ Kontrast & Farbwahl prüfen

- WCAG empfiehlt mindestens **4.5:1** für normalen Text
- Tools: [Contrast Checker](https://webaim.org/resources/contrastchecker/)

### ✅ Medien barrierefrei machen

- Alternativtexte für Bilder
- Untertitel für Videos
- Texttranskripte für Podcasts

---

## 5. Tools zur Prüfung von Barrierefreiheit

| Tool | Beschreibung |
|------|--------------|
| [axe DevTools](https://www.deque.com/axe/) | Browser-Plugin zur WCAG-Prüfung |
| [WAVE](https://wave.webaim.org/) | Visuelles Analyse-Tool von WebAIM |
| [Lighthouse (Chrome DevTools)](https://developers.google.com/web/tools/lighthouse/) | Automatischer Barrierefreiheitstest |
| [NVDA](https://www.nvaccess.org/) | Kostenloser Screenreader für Windows |
| [VoiceOver](https://support.apple.com/en-us/HT204390) | Eingebauter Screenreader auf macOS/iOS |

---

## 6. Relevante Richtlinien

- **WCAG 2.1 (Web Content Accessibility Guidelines)**  
  [https://www.w3.org/TR/WCAG21/](https://www.w3.org/TR/WCAG21/)

- **BITV 2.0 (Barrierefreie Informationstechnik-Verordnung, Deutschland)**  
  [https://www.bitvtest.de/bitv_test/bitv_2_0.html](https://www.bitvtest.de/bitv_test/bitv_2_0.html)

- **EN 301 549 (EU-Norm für barrierefreie IT-Produkte)**  
  [https://www.etsi.org/deliver/etsi_en/301500_301599/301549/](https://www.etsi.org/deliver/etsi_en/301500_301599/301549/)

---

## 7. Weiterführende Ressourcen

- 🌐 [WebAIM: Introduction to Web Accessibility](https://webaim.org/intro/)
- 🌐 [W3C Web Accessibility Initiative (WAI)](https://www.w3.org/WAI/)
- 📖 [Accessible Design Guide (MDN)](https://developer.mozilla.org/en-US/docs/Learn/Accessibility)
- 🎓 [Google's Accessibility Fundamentals (Free Course)](https://web.dev/learn/accessibility/)
- 📘 [Inclusive Design Principles (inclusive-components.design)](https://inclusive-components.design/)

---

**Let’s build an inclusive web – for everyone.**

