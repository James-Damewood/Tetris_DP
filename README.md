Solving Tetris using Dynamic Programming

Note: this version of tetris does not delete rows even if they are filled. This algorithm finds a suitible strategy for N pieces if one is possible.

For the DP, subproblems are the possible skylines of the board. For N pieces, Board of Height h and Width w. # subproblems = N*(H+1)^W

For each subproblem, we condsider all of the possible placements of the next piece = 4*W (including rotations)

Total runtime = N*W*(H+1)^W

Because this algorithm is exponential in w, the width of the board must be kept relatively small.

This implementation is based off the algorithm introduced in this lecture: https://www.youtube.com/watch?v=tp4_UXaVyx8

See Tetris.gif for an example game.

![me](https://github.com/Daisyliu6/Daisyliu6/blob/master/me.gif)
