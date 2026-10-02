# Greibach Normal Form (GNF) Converter

An interactive web application for converting Context-Free Grammars (CFGs) into **Greibach Normal Form (GNF)**.

The application provides a step-by-step visualization of the grammar transformation process and also includes a string membership tester to compare the original CFG with the converted GNF gramma

 **Project Overview**

Greibach Normal Form (GNF) is a standard form of Context-Free Grammars used in Formal Language and Automata Theory.

In GNF, productions generally follow the form:
A → aA₁A₂...Aₖ

The application performs the conversion through six major stages.

**GNF Conversion Pipeline**

**Step 1 — Null (ε) Removal**

Removes nullable productions and updates the grammar accordingly.

**Step 2 — Unit Removal**

Removes unit productions such as: A → B
and substitutes the productions of the referenced non-terminal.

**Step 3 — CNF Conversion**

Transforms productions into an appropriate Chomsky Normal Form representation before continuing the GNF conversion.

**Step 4 — Left Recursion & Ordering**

Handles direct and indirect left recursion and establishes the required variable ordering.

**Step 5 — Back-Substitution**

Performs substitution using ordered variables to transform productions toward terminal-leading form.

**Step 6 —  Z-Substitution & Final GNF**

Performs Z-variable substitution and enforces strict GNF formatting.
The final grammar follows the structure:A → a A₁ A₂ ... Aₖ

The application includes a String Membership Tester.

A user can enter a string and compare whether it is accepted by:

The original CFG
The converted GNF grammar

The application also reports whether the acceptance results are equivalent.

Example:Input: "abb"

Original Grammar: ACCEPTED
Final GNF Grammar: ACCEPTED
Language Equivalence: VERIFIED



 Technology      Purpose                    
 --------------   -------------------------- 
 HTML5            Application structure      
 CSS3             User interface and styling 
 JavaScript       GNF conversion logic       
 JavaScript DOM   Interactive UI             
 Git              Version control            
 GitHub           Source code hosting        
 GitHub Pages     Application deployment     

OPEN THE GNF CONVERTER APPLICATION
(https://swethatamarada.github.io/GNF-Grammar-Converter/)










