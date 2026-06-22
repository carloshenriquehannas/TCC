# Methods

This repository contains methodological artifacts, UML diagrams, and evaluation results related to the use of Large Language Models (LLMs) for generating and refining UML diagrams.

The materials are organized around a process that explores LLM-assisted diagram generation, formalizes guidelines, and evaluates the resulting diagrams across different system domains.

## Overview

The repository includes:

* Methodology activity diagrams describing the overall research/process flow.
* Exploratory PlantUML diagrams generated for a restaurant system.
* Formalized guidelines for generating UML use case, component, and class diagrams.
* Evaluation results of the guidelines applied to multiple example systems (system 1, system 2, system 3 and system 4).
* Source diagrams in PlantUML (`.puml`) and diagrams.net/draw.io (`.drawio`) formats.
* Rendered outputs in image/PDF formats, mainly under `out/` folders.

## Repository Structure

```text
Methods/
├── Auxiliary-Activity Diagrams/
│   ├── diagAtividades-Metodologia.puml
│   ├── diagAtividades-Metodologia-en.puml
│   ├── metodologiaApresentacao.drawio
│   └── out/
│       ├── diagAtividades-Metodologia.png
│       ├── diagAtividades-Metodologia-en.png
│       └── metodologiaApresentacao.pdf
│
├── Exploration of LLM for UML diagrams generation/
│   ├── casoUso-restaurante-*.puml
│   ├── componentes-restaurante-*.puml
│   └── diagramaClasses-restaurante-*.puml
│
├── Formalization of the Guidelines/
│   ├── diagAtividades-etapa3-casoUso*.puml
│   ├── diagAtividades-etapa3-componentes*.puml
│   ├── diagAtividades-etapa3-diagramaClasses*.puml
│   ├── diagBlocos*.drawio
│   └── out/
│
└── Evaluation Results of the Guidelines/
    ├── System1-Atletas/
    ├── System2-Biblioteca/
    ├── System3-RPG/
    └── System4-SmartMed/
```

## Main Methodological Flow

The methodology is represented as an activity diagram and follows these main steps:

1. Study of the Object-Oriented Analysis and Design (OOAD) subprocess.
2. Exploration of LLMs for UML diagram generation.
3. Formalization of guidelines.
4. Evaluation of the guidelines.
5. Diagram evaluation and refinement cycles.

A rendered version of the English methodology diagram is available at:

```text
Methods/Auxiliary-Activity Diagrams/out/diagAtividades-Metodologia-en.png
```

## Guideline Formalization

The `Formalization of the Guidelines` directory contains activity diagrams that describe structured prompting workflows for generating different UML diagram types.

### Use Case Diagram Guidelines

The use case guideline workflow includes:

* Collecting all system user stories.
* Generating actors and inheritance relationships.
* Correcting missing or inconsistent actors.
* Generating use cases actor by actor.
* Refining dependency relationships such as `include` and `extend`.

### Component Diagram Guidelines

The component guideline workflow includes:

* Listing possible components based on use case diagrams.
* Grouping similar components to improve cohesion.
* Generating PlantUML component code.
* Refining components and relationships according to use case semantics.

### Class Diagram Guidelines

The class diagram guideline workflow includes:

* Generating classes from use case and component diagram semantics.
* Adding inheritance relationships.
* Defining associations and multiplicities.
* Adding attributes based on real class characteristics.
* Applying corrective prompts when inconsistencies are found.

## Evaluation Systems

The guidelines were evaluated using four different systems:

### System 1 — Athletes

Includes use case, component, and class diagrams for a platform involving athletes, sponsors, representatives, clubs, posts, calendars, events, contracts, and performance reports.

### System 2 — Library

Includes diagrams for a library/reservation system involving system users, community members, librarians, administrators, rooms, equipment, reservations, availability, and notifications.

### System 3 — RPG

Includes diagrams for an RPG game system involving players, beginner and experienced users, tutorials, progression, rankings, inventory, moderation, persistence, and difficulty adjustment.

### System 4 — SmartMed

Includes diagrams for a healthcare/medication management system involving patients, doctors, technicians, operators, administrators, prescriptions, medication adherence, sensors, inventory, notifications, security, and interoperability.

Each evaluation system contains:

* Use case diagrams.
* Component diagrams.
* Class diagrams.
* Portuguese and English versions where available.
* Rendered PNG outputs under each system's `out/` directory.

## Diagram Formats

This repository uses the following formats:

| Format    | Purpose                                   |
| --------- | ----------------------------------------- |
| `.puml`   | PlantUML source files                     |
| `.drawio` | diagrams.net/draw.io editable diagrams    |
| `.png`    | Rendered diagram images                   |
| `.pdf`    | Rendered presentation or diagram document |

All files with `*-en.*`  represent english version.                         

## Suggested Usage

This repository can be used to:

* Study a methodology for LLM-assisted UML diagram generation.
* Reuse the formalized prompting workflows for new systems.
* Compare generated UML diagrams across different domains.
* Evaluate consistency between use case, component, and class diagrams.
* Maintain editable and rendered versions of UML artifacts.

## Notes

* Some directories and file names use Portuguese terms because part of the material was originally created in Portuguese.
* English versions are identified with the `-en` suffix where available.
* Rendered diagrams are stored in `out/` directories.
* The repository focuses on methodological and modeling artifacts, not executable application source code.

## License

No license file was identified in the provided project files. Add a license before distributing or reusing this repository publicly.

---

This README was generated by artificial intelligence.

