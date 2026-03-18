# neural-visual-lab
Neuronale Netze, Backpropagation und Transformer — interaktiv erklärt.Vom Forward Pass bis zu „Attention Is All You Need”. Mit Rotkäppchen.

## Was ist das hier?

Dieses Repository ist eine Sammlung von **interaktiven Browser-Visualisierungen**, die die wichtigsten Konzepte moderner KI erklären — ohne Vorkenntnisse, ohne Installations-Aufwand, direkt im Browser.

Entstanden als Begleitmaterial für Workshops, Schulvorträge und alle, die endlich *wirklich* verstehen wollen, was ein neuronales Netz tut.

-----

## 🗂 Inhalt

|Datei                             |Konzept                                    |Beschreibung                                                                                               |
|----------------------------------|-------------------------------------------|-----------------------------------------------------------------------------------------------------------|
|`01-forward-pass/neural-net.html` |**Forward Pass**                           |3-Layer-Netz mit einstellbaren Gewichten & Biases. Sieh in Echtzeit, wie sich der Output verändert.        |
|`02-backpropagation/backprop.html`|**Backpropagation & Gradient Descent**     |Trainiere ein Netz live auf XOR, AND, OR und Circle. Beobachte Loss-Kurve, Gradienten und Gewichts-Updates.|
|`03-transformer/transformer.html` |**Transformer — Attention Is All You Need**|Self-Attention, Multi-Head Attention und der vollständige Transformer-Block interaktiv erkundet.           |
|`04-stories/rotkaeppchen-nn.html` |**Rotkäppchen erklärt neuronale Netze**    |Ein neuronales Netz lernt, den Wolf zu erkennen — 6 Szenen, 6 Eingaben, 4 versteckte Muster.               |

-----

## 🚀 Schnellstart

Kein Build-System, kein npm, kein Server nötig.

```bash
git clone https://github.com/dein-name/neural-visual-lab.git
cd neural-visual-lab
open 01-forward-pass/neural-net.html
```

Oder einfach die gewünschte `.html`-Datei direkt im Browser öffnen.

-----

## 🎓 Lernpfad

Empfohlene Reihenfolge für Einsteiger:

```
1. Rotkäppchen        →  Intuition: Was tut ein Netz überhaupt?
2. Forward Pass       →  Mechanik: Wie fließt ein Signal durch?
3. Backpropagation    →  Lernen: Wie verbessert sich das Netz?
4. Transformer        →  Moderne KI: Was steckt hinter ChatGPT & Co.?
```

-----

## 💡 Kernkonzepte

### Was ist ein Forward Pass?

Eingabedaten fließen schichtweise durch das Netz. Jedes Neuron berechnet eine gewichtete Summe seiner Eingaben, addiert einen Bias und wendet eine Aktivierungsfunktion an:

```
z = Σ (wᵢ · xᵢ) + b
a = Aktivierung(z)    # z.B. ReLU oder Sigmoid
```

### Was ist Backpropagation?

Der Fehler (Loss) zwischen Vorhersage und Wahrheit wird rückwärts durch das Netz propagiert. Jedes Gewicht wird um einen kleinen Schritt in die Richtung angepasst, die den Fehler verringert:

```
w := w - η · ∂Loss/∂w
```

### Was ist Self-Attention?

Der Kern des Transformer-Modells. Jedes Token berechnet, wie stark es auf jedes andere Token achten soll:

```
Attention(Q, K, V) = softmax(QKᵀ / √dₖ) · V
```

-----

## 📖 Erklärungsguide für Laien

### Der eine Satz, der alles zusammenfasst:

> *„Ein neuronales Netz lernt Muster aus Beispielen — nicht durch Regeln, die jemand programmiert hat, sondern durch Fehler, die es selbst korrigiert.”*

### Häufige Fragen

**„Versteht das Netz wirklich?”**  
Nein — nicht im menschlichen Sinne. Es erkennt statistische Muster in enormen Datenmengen mit verblüffender Präzision. Irgendwo zwischen „reinem Muster-Matching” und „echtem Verstehen” liegt eine Grauzone, über die Forscher bis heute diskutieren.

**„Woher weiß es, was wichtig ist?”**  
Aus Millionen von Beispielen. Niemand hat die Gewichte programmiert — sie entstehen durch tausende Iterationen von Fehler messen → Gradient berechnen → Gewichte anpassen.

**„Warum braucht das so viel Strom?”**  
Weil für jedes Wort mit jedem anderen Wort gerechnet wird, in jeder Schicht, für jede Anfrage — Milliarden von Multiplikationen pro Sekunde.

**„Unterschied zu altem Google Translate?”**  
Früher: Wort für Wort, sequenziell, Kontext geht verloren. Heute: alle Wörter gleichzeitig, vollständiger Kontext, dramatisch bessere Qualität.

-----

## 🛠 Technologie

Alle Visualisierungen sind:

- **Reines HTML/CSS/JavaScript** — keine externen Dependencies
- **Offline-fähig** — funktioniert ohne Internet
- **Mobile-kompatibel** — läuft auf Tablets und Smartphones
- **Open Source** — frei verwendbar für Bildungszwecke

-----

## 📚 Weiterführende Ressourcen

|Ressource                                                                                                |Beschreibung                                    |
|---------------------------------------------------------------------------------------------------------|------------------------------------------------|
|[Attention Is All You Need](https://arxiv.org/abs/1706.03762)                                            |Das Original-Paper von Vaswani et al. (2017)    |
|[3Blue1Brown — Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)|Hervorragende visuelle Erklärungen              |
|[Andrej Karpathy — makemore](https://github.com/karpathy/makemore)                                       |GPT von Grund auf bauen                         |
|[The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)                       |Detaillierte visuelle Erklärung des Transformers|

-----

## 🤝 Beitragen

Fehler gefunden? Idee für eine neue Visualisierung? Pull Requests sind willkommen.

Besonders gesucht:

- Convolutional Neural Networks (CNN) Visualisierung
- LSTM / Recurrent Networks
- Embeddings & Vektorräume
- Übersetzungen in andere Sprachen

-----

## 📄 Lizenz

MIT License — frei verwendbar für Bildung, Workshops und Vorträge.  
Nennung freut uns, ist aber keine Pflicht.

-----

<div align="center">

**Gebaut mit ❤️ für alle, die KI wirklich verstehen wollen.**

*„Jede ausreichend fortgeschrittene Technologie ist von Magie nicht zu unterscheiden.”*  
— Arthur C. Clarke

</div>
