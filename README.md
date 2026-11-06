# synapsNOISE

**synapsNOISE** ist ein analoges Eurorack-Rauschmodul, das eine Vielzahl unterschiedlicher Rauschfarben sowie eine ansteuerbare „Grainy“-Shaper-Sektion bereitstellt. Das Modul wurde entwickelt, um von klassischem weißem Rauschen bis hin zu rauen, texturierten und CV-modulierbaren Rauschstrukturen alles zu liefern.

---

## Funktionen & Signalwege

* **Rauschfarben**: Bereitstellung verschiedener gefilterter Rauschspektren (Weiß, Rot, Pink, Blau, Violett).
* **Grainy-Sektion**: Spezieller Shaper-Zweig mit Dioden-Clipping und CV-Modulation zur Erzeugung von körnigen, raueren Rauschtexturen.
* **Mixer-Stufe**: Integrierter 6-Kanal-Summierer (basierend auf TL072) zum stufenlosen Mischen und Anpassen der Pegel an einem gemeinsamen Ausgang (`Mix Out`).
* **Eingangs- / Generator-Stufen**: Kombiniert Zener-Rauschen, Transistor-Rauschen und logikbasierte Rauschstrukturen (CD4093).

---

## Hardware-Struktur

Das Projekt ist modular im KiCad-Schaltplan aufgeteilt:
* `synapsNOISE.kicad_sch` (Hauptschaltplan)
* `noisesources.kicad_sch` (Rauschquellen)
* `rednoise.kicad_sch`, `pinknoise.kicad_sch`, `bluenoise.kicad_sch`, `violetnoise.kicad_sch` (Filterstufen)
* `grainyout.kicad_sch` (Grainy-Shaper & CV-Sektion)
* `mixer.kicad_sch` (Summierer und Ausgangsstufe)
* `power.kicad_sch` (Stromversorgung & Filterung)

---

## Produktion & Fertigung

Im Ordner `production/` befinden sich alle relevanten Daten für die Leiterplattenfertigung und Bestückung:
* Gerber- und Bohrdateien (`synapsNOISE.zip`)
* Stückliste (`bom.csv` / `bom.ods`)
* Bestückungspositionen (`positions.csv`)

---

## Lizenz & Rechtliches

Dieses Projekt ist Open-Source-Hardware und Open-Source-Software. Die jeweiligen Komponenten unterliegen den folgenden Lizenzen:

| Komponente | Lizenz | Beschreibung |
| :--- | :--- | :--- |
| **Hardware & Platinen** | [CERN OHL v2.0](https://ohwr.org/cernohl) | Gilt für Schaltpläne, PCB-Layouts und CAD-Dateien. |
| **Firmware & Code** | [MIT License](https://opensource.org/licenses/MIT) | Gilt für jeglichen Software- oder Skriptcode im Repository. |

*Entwickelt als Teil der Open-Source Eurorack-Initiative `synaps`. Bei Nachbau, Modifikation oder kommerzieller Nutzung sind die jeweiligen Lizenzbedingungen zu beachten.*
