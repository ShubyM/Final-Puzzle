# Zack's Solution
## Clarification
I, at one point, heard of this puzzle from Rik Sengupta (other Math Puzzles sections' professor), so I somewhat remember the basic idea.  
## Solution
Suppose you have everyone lined up such that person *i* has height *i*, so left to right you have *[10,9,8,...,3,2,1]*.
The general strategy should be something along the lines of having person 10 count the number of each color and guess their hat color as the one with the most instances; since they see 9 hats, you're guaranteed only 1 has the most instances.  This guess may be wrong (possibly using the 1 incorrect guess), but the rest should be correct based on the strategy.

With 10's guess made, 9 can look ahead and count, and whatever hat color (of theirs) would make 10's observation true, that is the hat color they would guess.  For example, if 10 said 'black' and 9 sees 2 white and 6 black, then 9 would guess 'black'.  Similarly, if 9 instead saw 4 white and 4 black, they would guess 'black' (as their black hat would be the tie-breaker).  

This strategy should work all the way down the line, as long as everyone remembers the colors said before them and keeps track of what has been said (in comparison to what they see in front of them).  As long as the first guess was accurate, everyone else should be able to see all the hats in front of them and hear all the hats behind them, making it easy for them to guess their hat color (based on 10's initial guess).
