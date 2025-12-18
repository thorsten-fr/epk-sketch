## Eingabeformat (EPK-Sketch)

Die EPK wird **zeilenweise in Textform** beschrieben.  
Jede Zeile beginnt mit einem Kürzel, gefolgt von einem Doppelpunkt (`:`) und dem Inhalt.

### Übersicht der Kürzel

| Kürzel | Bedeutung |
|------|-----------|
| `E:` | Ereignis |
| `F:` | Funktion |
| `K:` | Logischer Konnektor (`UND`, `ODER`, `XOR`) |
| `I:` | Informationsobjekt |

---

### Grundregeln der Eingabe

- Jede Zeile beschreibt **genau ein Element**
- Die Reihenfolge der Zeilen entspricht der **logischen Abfolge im Prozess**
- Ereignisse (`E`) und Funktionen (`F`) **wechseln sich ab**
- Konnektoren (`K`) stehen **zwischen mehreren gleichartigen Elementen**
- Informationsobjekte (`I`) beziehen sich auf die **zuletzt genannte Funktion**

---

### Beispiel: XOR-Verzweigung

```text
E: Gast möchte bezahlen
K: XOR
F: Gast zahlt bar
F: Gast zahlt mit Karte
