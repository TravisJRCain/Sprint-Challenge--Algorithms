#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) The runtime shown here is O(n). There is a linear increase with each step. The algorithm iterations reflect n directly. Ex) n=1 -> 1 iteration, n=2 -> 2 iterations, etc.


b) The runtime shown here is O(nlog(n)). For inputs n=1 -> 0 iterations, n=5 -> 15, n=10 -> 40, etc.


c) The runtime shown here is O(1), which is a constant runtime. However, if the function is modified with an else statement, for example, def bunnyEars(bunnies): if bunnies == 0: return 0 else: return 2 + bunnyEars(bunnies-1). The runtime would then become linear, O(n).

## Exercise II

I'd assume the floors are in a sorted list (0, 1, 2, 3, 4, etc.), therefore, I would use a binary search.

1. First, drop the egg at n/2 floor. n would be the total number of floors. Note result.
    - If the egg broke, eliminate all higher floors as points of interest.
    - If the egg did not break, eliminate all lower floors as points of interest.
2. Now, each time we drop an egg we do so from the middle of the range in which we have interest.
    - This means we can eliminate possible answers quickly.
    - This would be an O(log(n)) approach where n is the amount of floors. Therefore, the larger the building, the more floors we would need to consider.
