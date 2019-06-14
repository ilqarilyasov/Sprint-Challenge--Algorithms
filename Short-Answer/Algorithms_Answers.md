Add your answers to the Algorithms exercises here.

a)  a = 0
    while (a < n^3):
      a += n^2
    
    This will run just 2 time. O(1)
    First time 'a' is going to be 'n^2' and the next time 'a = n^4' and it's bigger than 'n^3' and loop will break

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

    n + n - 1 + n - 1 - 1 + 10 - 1 - 1 = 3n - 5 + 10 = 3n + 5 = n

    So this will run O(n) times