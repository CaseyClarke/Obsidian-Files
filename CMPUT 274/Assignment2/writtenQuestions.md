Question 1.
```python
def permutations(n):
    if n == 1:
        return [[1]]
		
    perms = []
    prev = permutations(n - 1)
    	
    for perm in prev:
        for i in range(n):
            permCopy = perm.copy()
            permCopy.insert(i, n)
            perms.append(permCopy)		
    return perms
```
Explanation:

The base case for the recursion is $n=1$, this returns 1 as there is only 1 way to arrange the list $[1]$, the reason why the code returns it in a double list is so that it is iterable by the double for-loop

For each recursive step in this function we take the list of permutations for $n-1$ and insert n at every location, thus creating a list with elements that are size n containing every permutation of $n$

Lets try the simple example of $n=3$, it is pretty easy to see that the list $[1,2,3]$ has 6 permutations
$$[[3, 2, 1], [2, 3, 1], [2, 1, 3], [3, 1, 2], [1, 3, 2], [1, 2, 3]]$$
Now lets go through the code and see if it does the same thing. 
Because we do the recursive step before anything else we go all the way down to $n=1$ which returns $$[[1]]$$Going one step up to $n=2$ we add n to every spot for every element in the previous step which returns $$[[2, 1], [1, 2]]$$Going one step up to $n= 3$ we add n to every spot for every element in the previous step which returns$$[[3, 2, 1], [2, 3, 1], [2, 1, 3], [3, 1, 2], [1, 3, 2], [1, 2, 3]]$$This is the same answer that we got at the start so the function is working correctly


Question 2.
```python
class StackUsingQueue:
    def init (self):
        self.queue = Queue()
        
    def push(self , element): 
        self.queue.enqueue(element)
        for i in range(len(self.queue) - 1):
            self.queue.enqueue(self.queue.pop())
        pass
        
    def pop(self):
        if not self.is_empty():
            return self.queue.pop()
        return None
        
    def top(self):
        if not self.is_empty():
            return self.queue.top()
        return None
		
    def is_empty(self):    
	    return len(self.queue) == 0 
             
    def size(self):
        return len(self.queue)
```