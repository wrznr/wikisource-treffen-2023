layout: true
  
<div class="my-header"></div>

<div class="my-footer">
  <table>
    <tr>
      <td style="text-align:right">Sächsische Landesbibliothek – Staats- und Universitätsbibliothek</td>
      <td>Würzner</td>
      <td style="text-align:right"><a href="https://www.slub-dresden.de/" style="visibility:hidden">www.slub-dresden.de</a></td>
    </tr>
    <tr>
      <td style="text-align:right">Universitätsbibliothek Mannheim</td>
      <td>Weil</td>
    </tr>
  </table>
</div>

<div class="my-title-footer">
  <table>
    <tr>
      <td style="text-align:left"><b>Stefan Weil</b></td>
      <td style="text-align:right"><b>Kay-Michael Würzner</b></td>
    </tr>
    <tr>
      <td style="text-align:left">Universitätsbibliothek Mannheim</td>
      <td style="text-align:right">SLUB Dresden</td>
    </tr>
    <tr>
      <td style="font-size:8pt"><b>14.Oktober 2023</b></td>
    </tr>
    <tr>
      <td style="font-size:8pt">2. Wikisource-Arbeitstreffen</td>
    </tr>
  </table>
</div>

---

class: title-slide
count: false

# Tesseract, Transkribus und Co
## OCR wird immer gebraucht

---

# Überblick

- Maschinelles Lernen am Beispiel der automatischen Texterkennung
- Werkzeugübersicht
- Diskussionsimpulse

---

class: part-slide
count: false

# Maschinelles Lernen am Beispiel der automatischen Texterkennung

---

# Kurze Einführung OCR

.cols[
.sixty[
- Bilderfassung ≠ Texterfassung
- **O**ptical **C**haracter **R**ecognition: Automatische Erfassung von Text in Bildern
- ursprünglich begrenzt auf Zeichenerkennung
- heute häufig Synonym für den gesamten Texterfassungsprozess
  + Bildvorverarbeitung
  + Layoutanalyse (OLR)
  + Zeilenerkennung
  + ...
]
.fourty[
<center><img src="https://upload.wikimedia.org/wikipedia/commons/9/9f/Codex_Manesse_127r.jpg" /></center>
]
]

---

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
]
.fourty[
<center>
<img src="https://cloud.google.com/static/vision/docs/images/sign_text.png" width="300px" />
<p style="font-size:4pt;">Image by Google, all rights reserved</p>
</center>
]
]

---

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
  - Nummernschilderkennung
]
.fourty[
<center>
<img src="img/anpr.svg" width="300px" />
<p style="font-size:4pt;">Image by Achim Raschka, CC BY-SA 3.0</p>
</center>
]
]

---

count: false

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
  - Nummernschilderkennung
  - Captcha-Umgehung
]
.fourty[
<center>
<img src="img/captcha.svg" width="300px" />
<p style="font-size:4pt;">Image by JD, CC BY-SA 2.0</p>
</center>
]
]

---

count: false

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
  - Nummernschilderkennung
  - Captcha-Umgehung
  - Schlüsselinformationsextraktion
]
.fourty[
<center>
<img src="img/deposit.svg" width="300px" />
<p style="font-size:4pt;">Image by Eluminary, CC BY-SA 2.0</p>
</center>
]
]

---

count: false

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
  - Nummernschilderkennung
  - Captcha-Umgehung
  - Schlüsselinformationsextraktion
  - Handschrifterkennung
]
.fourty[
<center>
<img src="img/transkribus.svg" width="300px" />
</center>
]
]

---

count: false

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
  - Nummernschilderkennung
  - Captcha-Umgehung
  - Schlüsselinformationsextraktion
  - Handschrifterkennung
  - Volltextdigitalisierung
]
.fourty[
<center>
<img src="img/beauvais_0.svg" width="300px" />
<p style="font-size:4pt;">Image by Uwe Springmann, CC BY-SA 4.0</p>
</center>
]
]

---

count: false

# Einsatzbeispiele

.cols[
.sixty[
- typische Anwendungen
  - Textspotting
  - Nummernschilderkennung
  - Captcha-Umgehung
  - Schlüsselinformationsextraktion
  - Handschrifterkennung
  - Volltextdigitalisierung
]
.fourty[
<center>
<img src="img/beauvais_1.svg" width="300px" />
<p style="font-size:4pt;">Image by Uwe Springmann, CC BY-SA 4.0</p>
</center>
]
]

---

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_raw.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_raw.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_opt.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_opt.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
    * **textflussunterbrechende** Elemente
        + Seitenzahlen
        + Kolumnentitel
        + Abbildungsunterschriften
        + Marginalien etc.
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
    * **textflussunterbrechende** Elemente
        + Seitenzahlen
        + Kolumnentitel
        + Abbildungsunterschriften
        + Marginalien etc.
    * **nichttextuelle** Elemente
        + Abbildungen
        + Tabellen etc.
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Komponenten eines einfachen OCR-Workflows

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
    * **textflussunterbrechende** Elemente
        + Seitenzahlen
        + Kolumnentitel
        + Abbildungsunterschriften
        + Marginalien etc.
    * **nichttextuelle** Elemente
        + Abbildungen
        + Tabellen etc.
- Texterkennung
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_text.svg" />
</p>
]
]

---

# Texterkennung: Zeichenorientierte Ansätze

.cols[
.seventy[
- Erkennung erfolgt *glyphenweise*
  - **Mustervergleich**: Vergleich der Zeichenbilder zu in einem „Setzkasten“ gespeicherten Glyphen **Pixel für Pixel**
  - **Merkmalsvergleich**: Zerlegung der Glyphen in vordefinierte, bedeutungstragende **Eigenschaften** wie *Einfärbung*, *Kurven*, *Linien* etc. und Vergleich zu Referenzmaterialien
]
.fourty[
<center><img src="img/char.svg" width="300px" /></center>
]
]

---

count: false

# Texterkennung: Zeichenorientierte Ansätze

.cols[
.seventy[
- Erkennung erfolgt *glyphenweise*
  - **Mustervergleich**: Vergleich der Zeichenbilder zu in einem „Setzkasten“ gespeicherten Glyphen **Pixel für Pixel**
  - **Merkmalsvergleich**: Zerlegung der Glyphen in vordefinierte, bedeutungstragende **Eigenschaften** wie *Einfärbung*, *Kurven*, *Linien* etc. und Vergleich zu Referenzmaterialien
]
.fourty[
<center><img src="img/char.svg" width="300px" /></center>
]
]
- *regelbasiertes Vorgehen*
    + **direkte** Abbildung von Referenzmaterial
    + Modellierung von Expertenwissen
- Zerlegung der Seite in *Zeilen* und *Zeichen* notwendig

---

# Texterkennung: Zeilenorientierte Ansätze

- Erkennung erfolgt *zeilenweise*
  1. **Skalierung:** einheitliche Höhe für alle Zeilen
  2. **Merkmalsextraktion**: Raster mit festgelegter Anzahl (horizontaler) Zeilen und variabler Anzahl (vertikaler) Spalten → Zeilen als Sequenzen binärwertiger Vektoren fixer Länge
<center><img src="img/grid.svg" width="800px"/></center>
- kontextsensitive Erkennung über *Übergangswahrscheinlichkeiten* der Vektoren
- Zerlegung der Seite in *Zeilen* notwendig
- Vorgehen robuster gegenüber Varianz durch Artefakte als zeichenorientierte Ansätze
- `Tesseract` (ab Version 4), `OCRopus`, `kraken`, `Calamari`
  + Einsatz *neuronaler Netze* für die Sequenzklassifikation

---

# Texterkennung: Zeilenorientierte Ansätze

- **Sequenzklassifikation**: zentrales Verfahren des maschinellen Lernens (cf. e.g. [Xing et al. 2010](https://www.cs.sfu.ca/~jpei/publications/Sequence%20Classification.pdf))
- basierend auf dem **Satz von Bayes**: `\(P(C|E) = \frac{P(E|C)\cdot P(C)}{P(E)}\)`
- Rezept
    + Man nehme
        * eine **sehr große** Liste **manuell annotierter** Daten und
        * einen **Trainingsalgorithmus**,
    + modelliere eine **`n:n`-Beziehung** zwischen Eingabe und Ausgabe,
        * e.g., jedes Eingabeelement (Buchstabe) wird auf eine Klasse abgebildet
    + induziere ein **statistisches Modell**,
    + und evaluiere dessen Qualität anhand von **Evaluationsdaten**

---

# Texterkennung: Zeilenorientierte Ansätze

- Übertragung auf OCR
    + Daten
        * https://htr-united.github.io/
        * manuell transkribierte Textzeilen
    + Kodierung `\(f: \mathbb{N}^{10}\rightarrow\mathbb{B}\)` 
      $$
      f(x[n]) = \begin{cases} 1 & \text{Pixel in Zelle $(x,n)$ schwarz} \\\\
      0 & \, \text{sonst}\end{cases}
      $$ 
    + Training
        * Zählen von Sequenzen aus Vektor-Buchstabenteil-Paaren
        * Repräsentation als OCR-Modell
        * Tesseract: [tesstrain](https://github.com/tesseract-ocr/tesstrain)
.cols[
.fifty[
```
  0123456789
0 1111111111
2 0000110000 
```
]
.fifty[
<center>
<img src="img/hi.png" style="width:150px"/>
</center>
]
]

---

# Texterkennung: Werkzeuge

.cols[
.fifty[
- viele verfügbare **OCR-Engines**
- [`Tesseract`](https://github.com/tesseract-ocr/tesseract)
    + ursprünglich von HP entwickelt
    + von Google übernommen und Open-Source gestellt
    + viele **mitgelieferte Modelle** (auch für „kleinere“ Sprachen)
    + ab Version 4 mit neuronalen Netzen
- [`OCRopus`](https://github.com/tmbdev/ocropy)
    + entwickelt von Thomas Breul
    + ebenfalls auf Basis neuronaler Netze
    + nur **wenige mitgelieferte Modelle**
    + weitere „Inkarnationen“
        * [`kraken`](http://kraken.re/), [`Calamari`](https://github.com/Calamari-OCR/calamari)
]
.fourty[
<p style="margin-top:-30px">
<img src="img/ocr.jpg" height="500px" />
</p>
]
]

---

# Texterkennung: Trainingsdaten

- fehlerfreies Referenzmaterial, sog. **Ground Truth**
    + Mapping von Zeilen-Bildern auf maschinenlesbaren codierten Text
    + entsprechend Konventionen (z.B. OCR-D-Richtlinien)
    + direkter Zusammenhang von Konventionen und Texterkennung
    + manuelle Erstellung (von Null oder aufbauend auf bereits erzeugtem Text, ggf. iterativ)
- aus Daten werden sog. **Modelle** erzeugt

<center>
<img src="img/gtlinecode.JPG" width="400px"/>
</center>

---

# Texterkennung: Trainingsdaten

- Lücken in Transkriptionsrichtlinien  
    * z.B. `"` vs. `“` oder `—` vs. `–` oder `⸗` vs. `-`
- zu wenige Beispiele für große Fonts und für spezifische Zeichen
- Wandel historischer Schreibweisen
    * z.B. am Übergang von Überpunkt zu Akut; Druckschwäche? 
      <img src="https://i.imgur.com/I1lloVk.png" width="400px" />
    * Absicht?
      <img src="https://i.imgur.com/uH5DbMC.png" width="200px" />
    * beschränkter Drucksatz?
      <img src="https://i.imgur.com/1Y3o6Ig.png" width="200px" />

---


# Texterkennung: Training und Evaluierung


- Umfang der GT-Daten
    + Fraktur: &gt; 16.000 Zeilen (1843–1911)
    + Antiqua: &gt; 16.000 Zeilen (1880–1934, 1950–)
- [Training von Modellen](https://github.com/bertsky/hsbcala) für Tesseract / Calamari …
    + auf Basis existierender Modelle
- Zeichenfehlerraten (CER) auf Test-GT:

|CER OCR|Abbyy Srv14† | Tesseract | hsb (Tess) | hsb (Cala) | hsb (multi) 
| ---------- | ---------- | -------- | ------------- |-------- |-------- |
|Fraktur‡  | 14,72% | 9,01% |0,56% | 0,45%  | 0,37% |
|Antiqua   |  ⁜  | 2,17%   |  0,89%  | 0,52%    | 0,48% |


<div style="font-size:8pt">
† Abbyy repräsentiert `ſ` als `s`<br/>
‡ v.a. Überpunkt vs. Akut<br/>
⁜ Stichproben mit Abbyy: bei Korrektur von ĕ (e breve) nach ě (e caron): < 1%<br/>
</div>

---

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
]
.fourty[
<p style="margin-top:-30px">
<img src="img/unzonned.jpg" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
]
.fourty[
<p style="margin-top:-30px">
<img src="img/unzonned.jpg" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
]
.fourty[
<p style="margin-top:-30px">
<img src="img/zonned.png" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
    + Illustration durch Farbe pro Segmenttyp
]
.fourty[
<p style="margin-top:-30px">
<img src="img/zonned.png" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
    + Illustration durch Farbe pro Segmenttyp
]
.fourty[
<p style="margin-top:-30px">
<img src="img/sem_sep.png" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
    + Illustration durch Farbe pro Segmenttyp
- Klassifikation der Pixel anhand ihrer **Umgebung** (i.e. Farbe im Original)
]
.fourty[
<p style="margin-top:-30px">
<img src="img/sem_sep.png" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
    + Illustration durch Farbe pro Segmenttyp
- Klassifikation der Pixel anhand ihrer Umgebung (i.e. Farbe im Original)
    + beliebig komplexe Schemata möglich
        * Text vs. Nichttext
]
.fourty[
<p style="margin-top:-30px">
<img src="img/sem_sep.png" height="500px" />
</p>
]
]

---

count: false

# *Layoutanalyse* per Pixelklassifizierung

.cols[
.fifty[
- Training auf manuell strukturierten Seiten
- jedes Pixel gehört in ein Segment
- jedes Pixel gehört zu einer Klasse
  + Illustration durch Farbe pro Segmenttyp
- Klassifikation der Pixel anhand ihrer Umgebung (i.e. Farbe im Original)
  + beliebig komplexe Schemata möglich
      * Text vs. Nichttext
]
.fourty[
<p style="margin-top:-30px">
<img src="img/text_sep.png" height="500px" />
</p>
]
]

---

# Layoutanalyse mit Eynollah

.cols[
.fifty[
- [quelloffenes](https://github.com/qurator-spk/eynollah) Werkzeug (cf. [Rezanezhad 2023](https://doi.org/10.1145/3604951.3605513))
    * kombiniert **maschinelles Lernen** und **Heuristiken**
    * trainierbar, frei verfügbare Basismodelle
    * Erkennung von:
        + Seitenrändern
        + Linien und Ornamentierung
        + Blocksegmentierung und Textfluss
        + Zeilensegmentierung
    * OCR-D-Wrapper
]
.fourty[
]
]

---

count: false

# Layoutanalyse mit Eynollah

.cols[
.fifty[
- [quelloffenes](https://github.com/qurator-spk/eynollah) Werkzeug (cf. [Rezanezhad 2023](https://doi.org/10.1145/3604951.3605513))
    * kombiniert **maschinelles Lernen** und **Heuristiken**
    * trainierbar, frei verfügbare Basismodelle
    * Erkennung von:
        + Seitenrändern
        + Linien und Ornamentierung
        + Blocksegmentierung und Textfluss
        + Zeilensegmentierung
    * OCR-D-Wrapper
]
.fourty[
<p style="margin-top:-30px">
<img src="img/segeynollah.jpg" height="500px" />
</p>
]
]

---

count: false

# Layoutanalyse mit Eynollah

.cols[
.fifty[
- [quelloffenes](https://github.com/qurator-spk/eynollah) Werkzeug (cf. [Rezanezhad 2023](https://doi.org/10.1145/3604951.3605513))
    * kombiniert **maschinelles Lernen** und **Heuristiken**
    * trainierbar, frei verfügbare Basismodelle
    * Erkennung von:
        + Seitenrändern
        + Linien und Ornamentierung
        + Blocksegmentierung und Textfluss
        + Zeilensegmentierung
    * OCR-D-Wrapper
]
.fourty[
<p style="margin-top:-30px">
<img src="img/segeynollah_fluss.jpg" height="500px" />
</p>
]
]

---

count: false

# Layoutanalyse mit Eynollah

.cols[
.fifty[
- [quelloffenes](https://github.com/qurator-spk/eynollah) Werkzeug (cf. [Rezanezhad 2023](https://doi.org/10.1145/3604951.3605513))
    * kombiniert **maschinelles Lernen** und **Heuristiken**
    * trainierbar, frei verfügbare Basismodelle
    * Erkennung von:
        + Seitenrändern
        + Linien und Ornamentierung
        + Blocksegmentierung und Textfluss
        + Zeilensegmentierung
    * OCR-D-Wrapper
- manuelle Korrektur
]
.fourty[
<p style="margin-top:-30px">
<img src="img/segeynollah_fluss.jpg" height="500px" />
</p>
]
]

---

count: false

# Layoutanalyse mit Eynollah

.cols[
.fifty[
- [quelloffenes](https://github.com/qurator-spk/eynollah) Werkzeug (cf. [Rezanezhad 2023](https://doi.org/10.1145/3604951.3605513))
    * kombiniert **maschinelles Lernen** und **Heuristiken**
    * trainierbar, frei verfügbare Basismodelle
    * Erkennung von:
        + Seitenrändern
        + Linien und Ornamentierung
        + Blocksegmentierung und Textfluss
        + Zeilensegmentierung
    * OCR-D-Wrapper
- manuelle Korrektur
]
.fourty[
<p style="margin-top:-30px">
<img src="img/seg_korr.jpg" height="500px" />
</p>
]
]

---

class: part-slide
count: false

# Diskussionsimpulse

---

# Diskussionsimpulse: Wikisource und OCR

- OCR profitiert von Trainingsdaten
- Wikisource profitiert von OCR
- **WS-Transkriptionsrichtlinien** erschweren Verwendung als Trainingsdaten
    + Zeilenfall inkl. Auflösung Worttrennung
    + stillschweigende Normalisierungen (insb. **ſ**)
        * Orientierung am DTA möglich?
    + **Text-Bild-Verknüpfung**
    + ...
- Problem ungleich relevanter für **Handschriftenerkennung**

---

# Diskussionsimpulse: kommerzielle OCR

- verschiedene Anbieter mit unterschiedlichem Hintergrund
    + lange Zeit **Abbyy** als Platzhirsch
        * Anschluss verloren?
    + IT-Firmen (Google CloudVision, Amazon Textract, MS Azure)
        * Fokus **Textspotting**
        * hohe Varianzrobustheit
    + Transkribus
        * ursprünglich aus der Wissenschaft
        * Fokus Handschriftenerkennung
- Probleme
    + **Anpassungsmöglichkeiten** stark eingeschränkt
        * Training, Kombination mit anderen Werkzeugen
    + **Datenhoheit**: „Was passiert mit meinen Eingaben?“
- Potenziale
    + enorme Power (Trainingsdaten, Rechnerkapazitäten)
    + Pflege und Weiterentwicklung „gesichert“

---

# Diskussionsimpulse: Layouterkennung

- größte offene Baustelle
    + komplexe Layouts
        * Zeitungen, Magazine, Formulare etc.
    + Textfluss
        * Rekonstruktion der intendierten Lesereihenfolge
    + logische Struktur
        * seitenübergreifende bzw. diskontinuierliche Phänomene
    + teilweise Abhängigkeit der Segmentklassifizierung vom Text
        * richtig wäre: Segmentierung, Texterkennung, Segmentklassifizierung
- DFG-Projekt *Robuste und performante Verfahren für die Layoutanalyse in OCR-D*
    + ab November 2023

---

class: part-slide

# Vielen Dank für Ihre Aufmerksamkeit!

<center>
<a href="https://wrznr.github.io/wikisource-treffen-2023/">wrznr.github.io/wikisource-treffen-2023</a>
</center>

---

class: part-slide
count: false

# Produktiver Workflow mit Werkzeugen aus OCR-D

---

# Produktiver Workflow mit Werkzeugen aus OCR-D

1. Erstellung Bilddigitalisate
2. Layoutanalyse mit `Eynollah`
3. ggf. manuelle Korrektur (Regionen und Textfluss)
4. Texterkennung mit `Tesseract` und `Calamari`
5. ggf. semiautomatische Textkorrektur
6. Konvertierung in Basis-TEI mit `mm2tei`
7. ggf. manuelle Korrekturen (insb. Worttrennung)
8. tiefergehende TEI-Auszeichnung (log. Struktur)

---

# Erstellung Bilddigitalisate

.cols[
.fifty[
<img src="img/scan.jpeg" height="400px" />
]
.fifty[
]
]

---

count: false

# Erstellung Bilddigitalisate

.cols[
.fifty[
<img src="img/scan.jpeg" height="400px" />
]
.fifty[
<img src="img/nd1967.jpg" height="500px" />
]
]

---

# Texterkennung

.cols[
.fifty[
- Prozesse zur **Vereinigung** verschiedener OCR-Ergebnisse in einen Volltext
    + **unterschiedliche Engines** bzw. Modelle haben **unterschiedliche Stärken** und machen unterschiedliche Fehler
    + **Extraktion** korrekter Textbestandteile [**aus mehreren OCR-Durchgängen**](https://www.researchgate.net/profile/John_Handley/publication/3776858_Improving_OCR_accuracy_through_combination_a_survey/links/0deec51e9c21900ab4000000/Improving-OCR-accuracy-through-combination-a-survey.pdf)
        * **Selbsteinschätzung** als Entscheidungskriterium
        * Integration vorhandener OCR ebenfalls möglich!
]
.fourty[
<p style="margin-top:-30px">
<img src="img/ocr.jpg" height="500px" />
</p>
]
]

---

# Semiautomatische Textkorrektur


.cols[
.fifty[
- Nachnutzung der freien Rechtschreibkorrektur [`hunspell`](https://hunspell.github.io/)
    * obersorbische Musterliste auf Basis von [`soblex`](https://soblex.de)
    * auch für Browser etc. nutzbar
- Identifikation und ggf. Korrektur nicht erkannter Wörter
    * einfaches, selbstgebautes Webinterface
    * gewisse Anzahl an **Falschnegativen**
        + unschön für die Bearbeitung
        + Integration in Lexikon
    * gewisse Anzahl an **Falschpositiven**
        + „Quasihomographe“ (*sto* vs. *što*)
]
.fourty[
<img src="img/hunspell.jpg" height="300px" />
]
]

---

# TEI-Konvertierung

- METS/ALTO: de-facto Standard für Repräsentation digitaler Volltexte in Bibliotheken
    * von der DFG empfohlene Formate für Digitalisierung
    * Anschluss an Präsentationssysteme
    * **Standoff Markup** für Text, Layout, Struktur → **seitenzentriert**
    * Anwendungsbeispiel: [Serbske Nowiny 23.3.1878 (DFG-Viewer)](http://digital.serbski-institut.de/ska-sn23031878_3u4)
- TEI-XML: de-facto Standard für Repräsentation digitaler Volltexte in der Wissenschaft
    * von der DFG empfohlenes Format für Korpora
    * Anschluss an Forschungsinfrastrukturen
    * **Inline Markup** für Text, Layout, Struktur → **dokumentzentriert**
- [`mm2tei`](https://github.com/slub/mets-mods2tei) als Brücke zwischen beiden Welten
    * Minimalauszeichnung
    * schrittweise manuelle Ergänzung

