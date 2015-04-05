# Knuths-algorithm-S
This is a method of randomly sampling n items from a set of M items, with equal probability; where M >= n and M, the number of items is unknown until the end. This means that the equal probability sampling should be maintained for all successive items > n as they become available (although the content of successive samples can change).

#####The algorithm
1. Select the first n items as the sample as they become available;
2. For the i-th item where i > n, have a random chance of n/i of keeping it. If failing this chance, the sample remains the same. If not, have it randomly (1/n) replace one of the previously selected n items of the sample.
3. Repeat #2 for any subsequent items.

