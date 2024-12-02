Question 1: Priority Queues:

```python
def push_with_priority(stack, priority, element):  
	temp_stack = []
	
	# 1)
	
	while len(stack) > 0:
		if stack.top()[0] > priority:
			temp_stack.push(stack.pop())
		else:
			break;
	
	# 2)
	
	stack.push((priority, element))
	
	# 3)
	
	while len(temp_stack) > 0:
		stack.push(temp_stack.pop())

```

Question 2: Binary Search Tree Operations:

a)
![[tree 2.png]]
b)
![[tree 3.png]]
c)

Using the Inorder Predecessor method of deletion we find the element we want to delete and replace it with the largest element in it's left subtree, in this case we replace it with 65 and leave the only other element (60) in the left subtree.

![[tree 1.png]]

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

Question 3: Sorting:

Task 1:

| Step          | Pivot | Left Partition            | Right Partition       |
| ------------- | ----- | ------------------------- | --------------------- |
| Initial Array |       | [8, -3, 7, -1, 10, 2,- 5] |                       |
| 1             | -5    | []                        | [-3, 7, -1, 10, 2, 8] |
| 2             | 8     | [-3, 7, -1 ,2]            | [10]                  |
| 3             | 2     | [-3,-1]                   | [7]                   |
| 4             | -1    | [-3]                      | []                    |
| Final Array   |       | [-5, -3, -1, 2, 7, 8, 10] |                       |

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

Task 2:
```python
def merge(S1, S2, S): 
	i = j = 0
	while i + j < len(S): 
		if j == len(S2) or (i < len(S1) and S1[i] < S2[j]):
			S[i+j] = S1[i]
			i += 1 
		else :
			S[i+j] = S2[j]
			j += 1
```
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

Task 3:
```python
def quick_sort_extra_storage(S,a,b):
	if a >= b:
		return
	pivot = S[b]
	left_partition = []
	right_partition = []
	for i in range(a,b):
		if S[i] < pivot:
			left_partition.append(S[i])
		else:
			right_partition.append(S[i])
			
	quick_sort_extra_storage(right_partition,0,len(right_partition) - 1)
	quick_sort_extra_storage(left_partition,0,len(left_partition) - 1)
	
	# Added lines Below
	
	S[a:b+1] = left_partition + [pivot] + right_partition
	
```
