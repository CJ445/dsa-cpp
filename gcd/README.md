You can do it naively by enumerating factors of both A and B and looking for largest common factor. This will take `O(sqrt(A+B))` time.


Solution Approach
We can use euclidean algorithm to find the GCD of two numbers. The algorithm is as follows:

gcd(A, B) = gcd(B, A mod B)
The complete pseudo code is as follows:

function gcd(A, B)
	while B ≠ 0
	   T := B
	   B := A mod B
	   A := T
	return A
The time complexity of this algorithm is `O(log(min(A,B)))` and space complexity is `O(1)`.
