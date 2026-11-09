# College of Computing Ontology (OWL)

An OWL ontology modeling the College of Computing at Umm Al-Qura University, built in Protégé. It includes a class hierarchy, object and data properties, axioms, individuals, reasoning, and SPARQL queries.

> Group project for the Knowledge Representation and Inference course (DS2203), Data Science Department, Umm Al-Qura University (2026).

## Ontology at a Glance
| Element | Count |
|---------|-------|
| Classes | 23 |
| Object properties | 8 |
| Data properties | 7 |
| Individuals | 21 |

## What Was Built
| Task | Details |
|------|---------|
| Class hierarchy (TBox) | 23 classes under `CollegeOfComputing`: Person (Student, FacultyMember, AdministrativeStaff), Building (Classroom, Labs, Offices), Program (GraduateProgram, UnderGraduateProgram), Course, Department, Event, Project, ResearchGroup |
| Object properties | `belongsToDepartment`, `teachesCourse` / `isTaughtBy` (inverse), `hasSubUnit` / `isSubUnitOf` (inverse), `locatedIn`, `offersProgram`, `memberOfCommittee` |
| Data properties | `courseName`, `courseCredits`, `departmentName`, `establishmentDate`, `hasProgramLevel`, `studentID`, `studentName` |
| Axioms | Cardinality restrictions, disjoint classes, and defined (equivalent) classes |
| Individuals (ABox) | 21 individuals: departments, courses, faculty, students, rooms, an event, and a project |
| Reasoning | Reasoner classification of the defined classes (GraduateProgram, UnderGraduateProgram, TaughtCourse) |
| SPARQL | Queries over events, faculty and the courses they teach, and facilities |

## Files
- `college_of_computing_ontology.owl`: the ontology

## How to Open
1. Install [Protégé](https://protege.stanford.edu/).
2. Open the `.owl` file with **File → Open**.
3. Start a reasoner from the **Reasoner** menu to see the inferred classes.

## Tools Used
Protégé, OWL 2, SPARQL

## Team
- Reem Omar Alotaibi
- Joud Alsaeedi
- Fay Salman Alzahrany
- Nada Almasoudi
