# NixieClock-Module
Module that abstracts the nixie tube clock to digital signals


## Signals
The following signals are meant to be multiplexed (one signal should be active at a time). You activate the signal by pulling it high.
N1 - First Nixie Tube
N2  - Second Nixie Tube
SEP - Separator
N3  - Third Nixie Tube
N4  - Fourth Nixie Tube

The following Truth Table shows how to interface with the K155NA1 IC.

| D | C | B | A | Res |
| --- | --- | --- | --- | --- |
| L | L | L | L | 0 |
| L | L | L | H | 1 |
| L | L | H | L | 2 |
| L | L | H | H | 3 |
| L | H | L | L | 4 |
| L | H | L | H | 5 |
| L | H | H | L | 6 |
| L | H | H | H | 7 |
| H | L | L | L | 8 |
| H | L | L | H | 9 |
