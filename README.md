# 2024-ryan-ms
This repository holds Nathan Ryan's Master's thesis.

## Guiding Questions
The questions that guide this work are:
1. What are the SWU requirements for TRISO fueled reactor transitions that incorporate the proposed LEU+ to HALEU scheme?
2. How quickly/often does it meet the energy demand (we would need to identify different limiting factors on the deployment in that case)?
3. If we have x growth of SMRs, how much TRISO do we need, and when do we exceed the demand?
4. What are the most sensitive facilities/parameters in the process?
5. What is the volume of waste and when will we run out of capacity in a Yucca mountain like facility?
6. What are the impacts of deployment schemes in FC scenarios, and what parts are realistic or unrealistic in each?
7. Is there a significant benefit in memory and time efficiency from altering the frequency that agents interact with the DRE?

I'm breaking this work up into parts: 1) replication of Amanda's method with
TRISO fuel; 2) DRE frequency evaluation; 3) waste and volume characterization
(different recycling technologies and latencies).

## Thesis Outline
1. Abstract.
   1. What is the research problem or question?
   2. What is the purpose of the study?
   3. What are the main conclusions or recommendations?
   4. What methods were used?
   5. What is the significance or implication of the findings?
2. Acknowledgments.
3. Introduction.
   1. Flexibility in generation and energy.
   2. Nuclear fuel cycle overview.
   3. TRISO overview.
      1. What is TRISO?
      2. How is it made?
      3. What is the current availability?
      4. What is the expected availability based on recent investments and promises?
      5. What forms might reactors use?
4. Background.
   1. Non-Equilibrium reactors.
      1. When are LWRs not operating at equilibrium?
      2. How might ARs operate differently?
   2. Cyclus.
      1. What is Cyclus? (What are the relevant functionalities of Cyclus?)
      2. What is Cycamore? (explain the specific archetypes used in the simulations)
      3. How does do these facilities interact with the DRE?
   3. Fuel cycle metrics.
      1. Isotopics.
      2. SWU.
      3. Energy production.
      4. Mass of fresh and used fuel.
      5. Questions:
         1. Why do we use this metric?
         2. Where in the fuel cycle is it impacted?
         3. How is it calculated?
         4. How does Cyclus treat this metric? (is that a valuable question, distinct from the above by relating to the software)
         5. What assumptions impact this metric?

5. Transition scenarios.
      1. Outline Amanda's methodology.
      2. Identify the intersection of scope and highlight the differences.
6. Deployment Scenarios (Results).
   1. Single reactor scenarios.
   2. Greedy deployment.
   3. Pre-determined deployment.
   4. Deployment cap.
   5. Random deployment.
   6. Initially random, then greedy deployment.
7. Sensitivity
8. Conclusions
   1. High-level overview: What were the guiding questions (not in question form), and how were they addressed?
   2. Limitations and assumptions.
   3. Future work.

## Amanda's Methodology
1. Metrics:
   1. energy generated,
   2. the number of advanced reactors deployed,
   3. the mass of enriched uranium, mass of feed uranium,
   4. SWU capacity required to produce the enriched uranium,
   5. and the UNF discharged from the reactors.
2. Sensitivity Study
   1. 
   2. Comparisons
      1. Build-share (x), transition start time (y), on SWU (z)
      2. Build-share (x), transition start time (y), on fuel mass (z)
      3. Build-share (x), burnup (y), on fuel mass (z)
      4. Build-share (x), percent of LWR lifetime extended (y), on fuel mass (z)

# ms-thesis-template
This repo holds the template for UIUC master's thesis.

- By Jin Whan Bae (Edited version of the uiucthesis2014 Package/Class)
- By Stephen Mayhew (Slightly) Edited version of the uiucthesis2009 Package/Class
- By Charles Kiyanda (Edited version of the uiucthesis07 Package/Class)
- by Tim Head (based on the Peter Czoschke version) (Edited version of the uiucthesis Package/Class)
- by Peter Czoschke (based on the original version by David Hull)

## Description
uiucthesis2018 is a LaTex package for formatting theses in the format required by the University of Illinois at Urbana Champaign.

## To compile:
Run `make` after making the appropriate edits to the `main.tex` file.