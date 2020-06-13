#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  a = 0 #constant O(1)
    while (a < n * n * n): #linear O(n)
      a = a + n * n 

    O(1) + O(n) ...drop lower order

    Total = O(n)



b) sum = 0 #constant #O(1)    # not count 
    for i in range(n): #O(n) 
      i += 1
      for j in range(i + 1, n): #O(n)
        j += 1
        for k in range(j + 1, n): #O(n)
          k += 1
          for l in range(k + 1, 10 + k): #O(1)
            l += 1
            sum += 1

        O(n) x O(n) x O(n) x O(1) = O(n^3)
     
     total = O(n^3)


c)  def bunnyEars(bunnies):
      if bunnies == 0: O(1) .... not count 
        return 0

      return 2 + bunnyEars(bunnies-1) #O(n)

     total = O(n)

## Exercise II
I's a summing there is a function that throws eggs!! Throw()
high_brake = true 
low_brake  = false 
low = 0 
high = n

While low_brake != high_brake: 
    high_brake = throw(high) #O(n) 
    low_brake = throw(low) #O(n) 
    f = low #O(1) 
    low += 1 #O(1) 
    high -= 1 #O(1) 
  return f

Time complexity: O(2^n)


