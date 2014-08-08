ObjCMazeSolver
==============

To use:
Open the project up in XCode and run. By default, the included sample.txt file is run. Feel free to modify the file to try out other mazes!

Scaling thoughts:
To have multiple bots search for the exit, start BFS from each start position with independent 'visited' flags for each bot. Once one bot finds the exit, the other bots keep searching until 1: they find the exits for themselves or 2: their search overlaps with a previously found shortest path.

At this point, the bots can begin following their shortest paths, doing a check each time to see if the next position is free from other bots and randomly deciding between multiple bots vying for a space.
