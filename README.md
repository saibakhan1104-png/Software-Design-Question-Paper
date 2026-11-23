# Software Design: Question Paper 

An outcome-based (OBE) question paper on **Software Design**, aligned to Bloom's Taxonomy and the BNQF cognitive domain. Every question is mapped to a Course Outcome (CO).

| Item | Detail |
|---|---|
| Full marks | 40 |
| Time | 1 hour |
| Sections | A (8 marks), B (16 marks), C (16 marks) |
| Bloom levels | K = Knowledge, U = Understanding, A = Application |


## Topics Covered

1. Design fundamentals (process, architectural vs detailed design)
2. Design principles (modularity, coupling, cohesion, information hiding)
3. Design quality and CK metrics (CBO, LCOM2, WMC)
4. Software architecture and architectural styles
5. Design patterns (GoF) and Fowler's enterprise patterns

## Course Outcomes (CO)

> These are assumed from the course topics. Replace them with your official COs if they differ.

| CO | Statement |
|---|---|
| CO1 | Explain the concepts, process and outcomes of software design |
| CO2 | Apply the principles of good design (modularity, coupling, cohesion, information hiding) |
| CO3 | Assess design quality using reviews and object-oriented metrics (CK suite) |
| CO4 | Describe and compare software architectural styles |
| CO5 | Explain and select design patterns (GoF and enterprise) for a given problem |

## Section A: Short Answers

Answer all. (8 × 1 = 8 marks)

| Q | Question | Marks | Bloom | CO |
|---|---|:---:|:---:|:---:|
| 1 | Define software design. | 1 | K | CO1 |
| 2 | Name the two steps of the software design process. | 1 | K | CO1 |
| 3 | What does low coupling mean? | 1 | K | CO2 |
| 4 | Define cohesion. | 1 | K | CO2 |
| 5 | What does the LCOM2 metric measure? | 1 | K | CO3 |
| 6 | List any two architectural styles. | 1 | K | CO4 |
| 7 | Under which GoF category (Creational, Structural or Behavioral) does the Adapter pattern fall? | 1 | K | CO5 |
| 8 | State in one sentence what the Domain Model pattern (Fowler) represents. | 1 | K | CO5 |

## Section B: Short Questions

Answer any 4 of 5. (4 × 4 = 16 marks)

| Q | Question | Marks | Bloom | CO |
|---|---|:---:|:---:|:---:|
| 9 | Distinguish between architectural (high-level) design and detailed design. | 4 | U | CO1 |
| 10 | Explain, with a suitable example, how high cohesion and low coupling improve maintainability. | 4 | U | CO2 |
| 11 | What does WMC measure? Explain the two ways it can be calculated. | 4 | U | CO3 |
| 12 | Describe the Pipes and Filters architectural style. Give one benefit and one liability. | 4 | U | CO4 |
| 13 | Differentiate between the Strategy and Template Method patterns in terms of intent and structure. | 4 | U | CO5 |

## Section C: Long Questions

Answer any 2 of 3. (2 × 8 = 16 marks)

### Q14 (CO3, Bloom: A)

Consider these classes:

- `OrderController` uses `OrderModel`, `OrderView` and `Logger`. `Validator` also uses `OrderController`.
- `OrderModel` has methods `m1()`, `m2()`, `m3()` and attributes `a`, `b`, `c`:
  - `m1()` uses `a` and `b`
  - `m2()` uses `b`
  - `m3()` uses `c`

(a) Calculate CBO for `OrderController`, counting coupling in either direction. **(2)**
(b) Calculate LCOM2 for `OrderModel`, showing the values of P and Q. **(4)**
(c) Interpret the LCOM2 result and suggest one refactoring. **(2)**

### Q15 (CO4, Bloom: U)

(a) Explain the Layered and Model-View-Controller (MVC) architectural styles, with the responsibility of each component or layer. **(5)**
(b) Compare the two styles on any two properties. **(3)**

### Q16 (CO5, Bloom: U)

For the Façade pattern, describe the following:

(a) Intent **(1)**
(b) Motivation, with a short example **(2)**
(c) Structure (participants and a labelled diagram) **(2)**
(d) Benefits and liabilities, including the "God class" risk **(3)**

## Blueprint Summary

| Section | Marks | Bloom level | COs covered |
|---|:---:|---|---|
| A | 8 | K (20%) | CO1 to CO5 |
| B | 16 | U (40%) | CO1 to CO5 (any 4 of 5 attempted) |
| C | 16 | U and A (40%) | CO3, CO4, CO5 (any 2 of 3 attempted) |

## Repository Structure

```
.
├── README.md
└── Software_Design_Question_Paper.docx
```
