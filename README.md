# Olivier Messiaen: _Mode de valeurs et d'intensités_ (1949)
 OpenMusic patch as an analysis/synthesis of Messiaen's _Mode de valeurs et d'intensités_

Design and Programming<br>
Antonio de SOUSA DIAS<br>
a.sousadias@belasartes.ulisboa.pt

- Current release: https://github.com/asousadias/Messiaen_ModeValeurs1949/files/4568286/messiaen_1949_mode_de_valeurs_et_d_intensites.zip

## Description:
The modeling of Olivier Messiaen's "Mode de valeurs et d'intensités" (1949) started as a challenge, regarding a remark by André Riotte, in one of his 1991 seminars I attended at IRCAM on computer analysis, arguing that analysis should be complemented by synthesis as a confirmation of the analytical process.<br/>
"Mode de valeurs et d'intensités" represents a very interesting example as, despite its historical importance for the development of integral serialism, in my opinion, the way the musical qualities (pitch, duration, intensity and attack mode) are linked to each other defines a mode rather than a series or even a scale.<br/>
Also, the difficulty of finding an efficient algorithm for generating automatically all events confirmed to me this pre-serial situation. But it also shows the possibility, through OM, of a modelization by successive approaches: for the establishment of the order of events, I have made descriptions mainly in extension (listing of all events one by one) and not in comprehension (e.g., the presentation of a general generation mechanism). The first being a description of a work, the second impliing a real analytical approach.<br/>
Also, one question I wanted to answer, raised by my curiosity was: "to what extent is the change in the order of the appearance of notes important for the recognition of this piece?"<br/>
Hence, you'll find the possibility of generating versions of "Mode de valeurs et d'intensités", playing with different ordering of the events of the work. This is possible by a  mode selection sort option that rearranges the modes elements present in the score in different ways:
- 0 - original event order by Messiaen;<br/>
- 1 - random order of mode elements;<br/>
- 2 - all mode elements sorted by position in each mode;<br/>
- 3 - mode elements arranged by serial exposition (an attempt).<br/>
As a comment, the simulation by ordering all the notes (option 2), bringing us closer to a musical surface closer to "minimal repetitive" music, very distant from the original surface.<br/>

## Setup and Operation
Unzip the _messiaen_1949_mode_de_valeurs_et_d_intensites.zip_ file and import the folder to your OM environment.<br>
- Launch the patch \__mode\_de\_valeurs\_tot_ or the simplified version \__mode\_de\_valeurs_.
- Evaluate the patch.

## Patch List
- _mode_de_valeurs_tot.omp - main patch:
- _mode_de_valeurs.omp - simplified main patch

### subsidiary patches:
- constr_rtm.omp - constructs the rythm figures for each voice
- modes_prep.omp - organizes each mode elements by a list of (pitch length velocity channel)
- modes.omp - the three modes setup (pitches, duration and attack mode)
- seq_fin_ind.omp - prepare list of mode elements to fill chord-seq object
- seq_fin.omp - prepare list of lists of mode elements to fill chord-seq objects
- serie_mode.omp - subsidiary patch to seq_fin_ind.omp and seq_fin.omp


## Score and References
The score for _Mode de valeurs et d'intensités_ is edited by Éditions Durand et Cie.<br>

For information about use, issues and discussion, see:<br>
- Sousa Dias, A. (2005). _L'Objet Sonore: Situation, Évaluation et Potentialités. Un paradigme pour la création d'outils de composition musicale_. Université Paris 8.<br>

## Revision history:
- 2020 - minor changes and revision for release in Github and compatibility with OM 6.16.
- 2005 - first release version Sousa Dias (2005).
- 2003 - first personal experiments.

## Disclaimer:
These patches are distributed in the hope that they will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.<br>

Universidade de Lisboa, Faculdade de Belas-Artes<br>
Largo da Academia Nacional de Belas-Artes<br>
1249-058 Lisboa, Portugal<br>
http://www.belasartes.ulisboa.pt/

www.sousadias.com
