# Assignment 3, Part 1 - Running Time

### Question 1
Compute the (tightest) Big O running time bound of the following scripts:

```
for i in range(N):
    for j in range(N^2):
        print(i + j)
```

Select one:
1. O(1)
2. O(Log N)
3. O(N)
4. O(N Log N)
5. O(N^2)
6. O(N^3)
7. O(2^N)

### Question 2
```
i = N
j = 1
while j<i:
    i *= 100
    j *= 101
```

Select one:
1. O(1)
2. O(Log N)
3. O(N)
4. O(N Log N)
5. O(N^2)
6. O(N^3)
7. O(2^N)

### Question 3
```
i = 0
j = 1
while i<N:
    for k in range(j):
        i += 1
    j *= 2
```
Select one:
1. O(1)
2. O(Log N)
3. O(N)
4. O(N Log N)
5. O(N^2)
6. O(N^3)
7. O(2^N)

### Question 4
```
def func(i):
    if i<1:
        return 1
    else:
        return func(i-1) + func(i-1) 
print(func(N))
```
Select one:
1. O(1)
2. O(Log N)
3. O(N)
4. O(N Log N)
5. O(N^2)
6. O(N^3)
7. O(2^N)