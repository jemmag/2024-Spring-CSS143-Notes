# Notes Template
### Date: 4/29/24
## Key Concepts

## Notes
* Complexity
     * aka "Cost" - think about complexity as COST
          * Time
          * Resources
               * CPU
               * Disk
               * Network
               * Power (electricity, for running and cooling) 
     * ...

## In-Class Exercises
### Exercise 1
* Need to cross the bridge at night with animals and we have a lamp that only works for *17 min*. Will we make it?
* Up to 2 pets can cross simultaneously (so not all 4 can go)
* One needs to come back to bring the lamp as well so the other one can use it
* Walk at the slowest pet's pace
     * Cat - 10 min
     * Bird - 5 min
     * Dog - 2 min
     * Bunny - 1 min
* Example: max(1, 5) - 5 min to go across the bridge since it's the slowest
* Question: Can we all cross the bridge within 17 min?
* Thought Process
     * Cannot do within 17 min
     * Bunny carries the lamp - 1 min
          * Bunny + Cat - max(1, 10) - 10 min
          * Bunny goes back - 1 min
          * Bunny + Bird - max(1, 5) - 5 min
          * Bunny goes back - 1 min
          * Bunny + Dog - max(1, 2) - 2 min
     * Total: 10 + 1 + 5 + 1 + 2 = 19 min total
     * Possible strategy: Dog and Bird goes together - CORRECT AND SHORTEST ANSWER !
          * Dog + Bird - max(5, 10) - 10 min
          * Bunny - 1 min
          * Bunny back - 1 min
          * Bunny + Dog - max(1, 2) - 2 min
     * TOtal: 10 + 1 + 1 + 2 = 14 min
 
### Exercise 2 - Helps with the homework
Weighing 9 boxes
* 9 boxes, same size, equally heavy - except for one, which is a little heavier
* With a pair of balance scales, how to identify the heavier box?
     * 4 on each side - if it's equal then no need to measure (extra box is the heavier)
     * if it's not equal, one side is probably heavier then that limits it
     * take a box off from each side - if one side is still heavier then you remove another pair of boxes
     * if the side gets lighter or if there is one left on one side, then you found the heavier box
     * Total: 1 or 3 times
* This is similar to Binary Search 
  
## Code Snippets
Include relevant code snippets discussed in the lecture
```java

# Example Python code
public static void main(String[] arr){
}

```

## Questions (Things I didn't understand)
* What's a variable?
     * Notes:
     * To be resolved by: end of 2nd week by talking to the teacher after lecture

## TODOs
- [ ] Go over code we did in class
- [ ] Start working on homework 3. **DUE: 5/5 (Sun)**
