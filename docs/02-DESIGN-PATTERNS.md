# Design Patterns

Poetry office nutzt wo möglich und sinnvoll Design Pattern
---

# Composite

                 BDocumentNode
                       |
        +--------------+--------------+
        |                             |
     Group                       Paragraph
        |
   +----+----+
   |         |
 Image     Chart

Der gesamte Dokumentbaum basiert auf Composite.

---

# Command

            BDocumentCommand
                     |
      +--------------+--------------+
      |              |              |
   Insert         Delete          Move

Alle Änderungen erfolgen über Commands.

Nutzen:

- Undo
- Redo
- Makros
- Scripting

---

# Visitor

                 Visitor
                    |
      +-------------+-------------+
      |             |             |
   Render       Export       Print

Verhalten wird erweitert,
ohne den Objektbaum zu verändern.

---

# Observer

                  BDocument
                       |
          +------------+-----------+
          |                        |
      Renderer               Editor

Änderungen am Dokument
erzeugen Ereignisse.

---

# Adapter

                  Adapter
                      |
      +---------------+---------------+
      |               |               |
    SumIt         Replicant         SVG

Adapter verbinden Fremdsysteme
mit dem Dokumentmodell.

---

# Factory

                 NodeFactory
                       |
      +----------------+----------------+
      |                |                |
 ParagraphNode   ImageNode      ChartNode

Neue Node-Typen können registriert werden,
ohne den Core anzupassen.

---

# Strategy

                  Strategy
                      |
      +---------------+---------------+
      |               |               |
    Writer      Presentation      Diagram

Verschiedene Anwendungen
können auf demselben Dokumentmodell basieren.

---

# Später möglich

- Flyweight
- State
- Memento
