#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)
    O(N)
    As N grows, A only slows down behind it by one exponent. This means the relative distance, while fast, will not grow fast enough to justify a higher complexity. It also has no way to lower our initial set, so it can't go lower.

b)
    O(N^2)
    Looped secdtions of code. Each of them are involving N. Classic N^2 case.

c)
    O(N)
    while this does have much higher space complexity, time complexity is only limited to what is essentially a for/while loop. No way to reduce the complexity and none to increase.


## Exercise II

In essence, this is a search. The quickest way, in this case, is to cut down your search area as fast as possible. If you had an egg limit, you'd have to change your algorithm a bit, but in this case, you are not limited. As such, your fastest method would be:

go to the n//2 floor
drop an egg and see if it breaks
if it survives, set the current floor as "ground" and adjust N accordingly.
if it breaks, set the current floor as N
repeat until N breaks your egg but N-1 does not.

Each time you drop the egg, you will be reducing your search area by half. As such, this runs in O(lg N) time.
