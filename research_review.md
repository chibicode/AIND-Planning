## Development 1: Robot Research, and STRIPS

During the late 1960s and early 1970s, researchers at the SRI AI Lab were working on a project: developing a mobile robot that could navigate and push objects around in a multi-room environment. The robot essentially had a cart which could push the boxes from one place to another, and a camera. It required visual scene analysis, planning, and converting the plans to actions. (Nilsson [11]).

This led to the development of A* algorithm, introduced in 1968 (Hart et al.). And this also led to STRIPS (Fikes and Nilsson, 1971), the first major planning system. STRIPS was developed by SRI to solve problems faced by robots in re-arranging objects and in navigating. Such class of problems was much more complex than puzzles and games, where a state can be stored in a matrix or a list.

## Development 2: ADL

ADL (Action description language) is an advancement of STRIPS, developed by Edwin Pednault in 1987. Unlike STRIPS:

- ADL assumes that everything not occurring in the conditions is unknown (instead of being assumed false).
- Negative literals and disjunctions are allowed.
- In goals, quantified variables are allowed.
- Conditional effects are allowed.
- Has support for equality and types.

ADL was developed because STRIPS was not suitable to model many real world applications, such as actions whose effects depend on the situations in which they are performed.

## Development 3: PDDL

PDDL (Planning Domain Definition Language) was developed by Drew McDermott and his colleagues in 1998 in order to make the 1998/2000 International Planning Competition (IPC) possible. At this point, there were many formalizations, including ADL, The SIPE-2 formalism, The Prodigy-4.0 formalism, The UMCP formalism, The Unpop formalism, and the UCPOP formalism. The goal was to come up with a standard langauge to encourage sharing of problems and algorithms, and allow meaningful comparison of the performance of planners.

PDDL led to many extensions, including PDDL+, NDDL, MAPL, OPT, PPDDL, APPL, RDDL, and MA-PDDL.

## References

- Richard E. Fikes, Nils J. Nilsson (Winter 1971). "STRIPS: A New Approach to the Application of Theorem Proving to Problem Solving" (PDF). Artificial Intelligence. 2 (3–4): 189–208
- P.E. Hart, N.J. Nilsson and B. Raphael, A formal basis for the heuristic determination
of minimum cost paths, 1EEE Trans. Syst. Sci. Cybern. 4 (2) (1968) 100-107
-  N.J. Nilsson, Shakey the Robot, SRI Tech. Note 323, Menlo Park, CA (1984).
- Fikes, Richard E., and Nils J. Nilsson. "STRIPS, a retrospective." Artificial Intelligence 59.1 (1993): 227-232.
-  McDermott, Drew; Ghallab, Malik; Howe, Adele; Knoblock, Craig; Ram, Ashwin; Veloso, Manuela; Weld, Daniel; Wilkins, David (1998). "PDDL---The Planning Domain Definition Language". Technical Report CVC TR98003/DCS TR1165. New Haven, CT: Yale Center for Computational Vision and Control.
- Wikipedia on ADL: https://en.wikipedia.org/wiki/Action_description_language
- Wikipedia on PDDL: https://en.wikipedia.org/wiki/Planning_Domain_Definition_Language
