# The Game of Life 

The Game of Life (an example of a cellular automaton) is played on a two-dimensional rectangular grid of cells. Each cell can be either dead or alive. The status of each cell changes each turn of the game (also called generation) depending on the statuses of that cell's 8 neighbors – neighbors of a cell are cells that touch that cell, either horizontal, vertical, or diagonal from that cell.

The initial pattern is the first generation. The second generation evolves from applying the rules simultaneously to every cell on the game board – i.e. births and deaths happen simultaneously. Afterwards, the rules are iteratively applied to create future generations. 

For each generation of the game, a cell's status in the next generation is determined by a set of rules:
* If the cell is alive, then it stays alive if it has either 2 or 3 live neighbors.
* If the cell is dead, then it springs to life only in the case that it has 3 live neighbors.
    
There are, of course, as many variations to these rules as there are different combinations of numbers to use for determining when cells live or die. Conway tried many of these different variants before settling on these specific rules. Some of these variations cause the populations to quickly die out, and others expand without limit to fill up the entire universe, or some large portion thereof. The rules above are very close to the boundary between these two regions of rules, and knowing what we know about other chaotic systems, you might expect to find the most complex and interesting patterns at this boundary, where the opposing forces of runaway expansion and death carefully balance each other. 

<img width="1399" alt="gol-conway" src="https://user-images.githubusercontent.com/83437383/118737287-c5539780-b801-11eb-9ca4-042bed41ebdc.png">

> Output example

Conway carefully examined various rule combinations according to the following three criteria:
* There should be no initial pattern for which there is a simple proof that the population can grow without limit.
* There should be initial patterns that apparently do grow without limit.
* There should be simple initial patterns that grow and change for a considerable period of time before coming to an end.
