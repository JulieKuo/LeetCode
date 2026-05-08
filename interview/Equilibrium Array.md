#### Question
Write a function to compute the equilibrium index for an input array of size N, or return -1 if no such index exists.

#### Clarifying Questions
Candidates may ask some or all of the following questions to clarify:

- What is the "equilibrium index"?
    - Equilibrium index of an array is an index such that the sum of all elements at lower indexes is equal to the sum of all elements at higher indexes.
- What if there is no index that satisfies the equilibrium index property?
    - Then your function should return -1.
- Are the values in the array integers?
    - Yes, all the values in the input array are integers.
- Can the array be mutated to yield a valid equilibrium index?
    - No, the input array should not be changed.
- What if the input array is empty?
    - An empty array has no equilibrium index, so your code should return -1.
- What if there are multiple equalibrium indicies?
    - Return the lowest such index.

#### Examples
If the students asks for an example, offer this:

```
Input: A[] = {-7, 1, 5, 2, -4, 3, 0}
Output: 3
```
3 is the lowest equilibrium index, because: (A[0] + A[1] + A[2]) = (A[4] + A[5]+ A[6]). Note that 6 is also an equilibrium index, but is not the lowest.

The following examples may be provided in response to more specific requests:

```
Input: B[] = {1, 2, 3}
Output: -1
```
No equilibrium index exists for B.

```
Input: C[] = {5,1,1,1,1,1,1}
Output: 1
```
1 is the only equilibrium index, because C[0] = (C[2] + C[3] + C[4] + C[5] + C[6]).

```
Input: D[] = {1, 0, 0, 0, 1}
Output: 1
```
Mutliple equalibrium indicies (1, 2, and 3). Returns the lowest such index.

```
Input: E[] = {100}
Output: 0
```
For a single-element array, the result is 0.

```
Input: F[] = {}
Output: -1
```
Returns -1 per clarifying questions above.

```
Input: G[] = {1, -1, 100}
Ouput: 2
```

#### Solution
- [724. Find Pivot Index](../724.%20Find%20Pivot%20Index.ipynb)
- [1991. Find the Middle Index in Array](../1991.%20Find%20the%20Middle%20Index%20in%20Array.ipynb)