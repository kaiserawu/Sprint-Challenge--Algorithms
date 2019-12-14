#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) The function effectively adds n^2 to a running sum until it becomes greater than n^3. As such, it takes n additions of n^2 to equal n^3, so the run time will be O(n).


b) The for loop runs at a linear scale, while the inner while loop multiplies j at an exponential scale since the value is doubling every time. Since the exponential rate is making the function run faster, the run time of the while loop is logarithmic, making the total run time O(nlog(n))


c) Bunnies is being decremented linearly at each recursive step, so the total run time is O(n)

## Exercise II

One strategy would be to use a binary search method and find the right floor by testing at half of the remaining height. The initial bounds are from 1 to n. You'd start by dropping an egg off of floor n/2, then if it broke, you'd know the upper bound is now n/2, so your range changes to 1 to n/2, and you'd drop the next egg halfway between those floors, i.e. floor n/4. Similarly, if the egg doesn't break, the bounds change to being from n/2 to n, and you'd drop the egg halfway, or at floor 3n/4. Repeat this until you find floor f. Since the range is halved each time, the time complexity is O(log(n))