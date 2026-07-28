# Future Extensibility

## Ziel

Neue Anwendungen sollen auf Basis
von BDocument entstehen können,
ohne den Core zu verändern.

---

# Mögliche Anwendungen

## Office

- Writer
- Spreadsheet
- Presentation

---

## Modellierung

- ProjectConceptor Nachfolger
- UML
- BPMN

---

## Wissensmanagement

- Mindmaps
- Wissensgraphen
- Notizsysteme

---

## Technische Anwendungen

- CAD
- Schaltpläne
- Layoutsysteme

---

# Erweiterungen

## Plugins

Neue Node-Typen sollen nachladbar sein.

Beispiele:

- FormulaNode
- MarkdownNode
- SQLNode
- ChartNode

---

## Automation

Später:

- HEY
- Makros
- Skripting
- Batch Verarbeitung

---

## Compound Documents

Dokumente können andere Dokumente:

- einbetten
- referenzieren
- wiederverwenden

---

## Grundsatz

Der Core kennt nur:

- BDocument
- BDocumentNode
- BDocumentCommand
- BDocumentVisitor

Alles Weitere wird erweitert.
