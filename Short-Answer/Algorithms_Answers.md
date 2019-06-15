Add your answers to the Algorithms exercises here.

## Exercise I

a)  a = 0
    while (a < n^3):
      a += n^2
    
    This is going to run linear time. Answer: O(n)

b)  sum = 0
    for i in range(n):
      i += 1                                //n
      for j in range(i + 1, n):
        j += 1                              //n - 1
        for k in range(j + 1, n):
          k += 1                            //n - 1 - 1
          for l in range(k + 1, 10 + k):    //10
            l += 1                          //1
            sum += 1                        //1

    n * (n - 1) * (n - 1 - 1) * 10 - 1 - 1 = n^3

    So this will run O(n) times

c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)

  This will run O(n) times


## Exercise II

n: story building
n: eggs
f: floor number

if f =< drop_off_floor then egg is broken
if f > drop_off_floor then egg is not broken

I would use binary search. To find out the break-even. 
Lets say we have 20 story and 30 eggs. I would drop an egg from 10th floor 
and see if it's broken or not. If it's broken I would decrease the number to 5
and keep going.

This algorithms time complexcity would be O(log n)