Add your answers to the Algorithms exercises here.

    Exercise 1. 
        a). although the upper limit is set at n^3, the counter grows at a rate of n^2, which makes the runtime actually only take --> O(n).

        b). since x isnt specified
            1st case -->  this wont run since x is undefined and in that case, O(1) --> O(1)
            2nd case -->  this will only run until it is lower than x, if x > 0 then that is O(logn) since the counter is approaching the limit at a rate faster than n but slower than n^2  --> O(logn)
            3rd case -->  if x < 0, dividing the coutner by 2 will never make the counter drop below 0 which will lead to an infinite loop --> O(infinite)

        c). the inner most loop will run 8 times consistently, the middle loop will also run 8 times consistently for a total of 64 consistent loops per sqrt(n)/2 so the answer is --> O(n^.5)

        d). the inner most loop will always run n times, but it will only occur at a logn number of times, so the time complexity would be --> O(n logn)

        e). inner most loop is consistent 10, middle 2 loops are both logn, outer loop is n. --> O(n logn^logn)
            logn * logn should make it logn^logn? i believe

        f). counter goes down by 1 each time so it will run n times, --> O(n)

        g). this will just iterate through an n where n is the length of the array so --> O(n)

    Exercise 2.
        a). const jBox = [array[0],0];
            const iBox = [array[0],0]; also initialed at 0 because >= , if > then [array[1],1]
            loop through array
            if a value is larger than jBox[0] && index is >= iBox[1], replace jBox[0,1] with [largest, index]
            if a value is smaller than iBox[0] && index is <= jBox[1], replace iBox[0,1] with [smallest, index]
            the [0] slot will track largest in jBox and smallest in iBox
            the [1] slot will make sure j >= i
            after 1 iteration, return jBox[0] - iBox[0] (largest - smallest) for max value while condition is kept true
        
        b). 1/2 system
            left side --> n thru pivot, pivot === n/2, right side --> pivot thru end
            at pivot, throw egg 
                if it breaks, go to the right side (less than n/2)
                else go to the left side (greater than n/2)
                repeat 1/2 system where pivot is new n

    Exercise 3.
        a). if the array is sorted, there will never be a less quicksort so this would function like a memoized recursive function and will just have a series of destructing the array into single units and then rejoining them back together sooo O(n logn)

        b). even if the middle most value is always the pivot, you would still need to split the array down to single units before rejoining in order so there will still have the runtime of O(n logn)