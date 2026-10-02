# Greibach Normal Form (GNF) Converter

An interactive web application for converting Context-Free Grammars (CFGs) into Greibach Normal Form (GNF).

#Live Demo

 [OPEN THE GNF CONVERTER APPLICATION](https://swethatamarada.github.io/GNF-Grammar-Converter/)

Click the link above to directly open and use the application.

Features

- Interactive CFG input
- CFG to GNF conversion
- Six-step transformation pipeline
- Null removal
- Unit production removal
- CNF conversion
- Left recursion removal
- Back-substitution
- Final GNF
- String membership testing

GNF Conversion Pipeline

Step 1 — Null (ε) Removal

Removes nullable productions and updates the grammar accordingly.

Step 2 — Unit Removal

Removes unit productions such as: A → B and substitutes the productions of the referenced non-terminal.

Step 3 — CNF Conversion

Transforms productions into an appropriate Chomsky Normal Form representation before continuing the GNF conversion.

Step 4 — Left Recursion & Ordering

Handles direct and indirect left recursion and establishes the required variable ordering.

Step 5 — Back-Substitution

Performs substitution using ordered variables to transform productions toward terminal-leading form.

Step 6 — Z-Substitution & Final GNF

Performs Z-variable substitution and enforces strict GNF formatting. The final grammar follows the structure:A → a A₁ A₂ ... Aₖ

A user can enter a string and compare whether it is accepted by:

The original CFG The converted GNF grammar

The application also reports whether the acceptance results are equivalent.

Example:Input: "abb"

Original Grammar: ACCEPTED Final GNF Grammar: ACCEPTED Language Equivalence: VERIFIED

 Technologies Used

- HTML5
- CSS3
- JavaScript
- Git
- GitHub Pages
