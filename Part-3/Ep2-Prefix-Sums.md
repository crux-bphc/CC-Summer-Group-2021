Part 3 Episode 2/3: Prefix Sums
=====

Given an array `A` of `n` elements, prefix sums are a very powerful technique that allows you to calculate the sum of any range of elements `[l, r]` for `1 <= l <= r <= n` in `O(1)` constant time with the help of `O(n)` pre-processing.

The trick is to pre-calculate in another array `prefix`, of cumulative sums, such that for each `i` from `1 to n`, `prefix[i]` stores the sum a[1] + a[2] + ... + a[i]. Then, the sum of elements in the range `[l,r]` can be easily found out as `prefix[r] - prefix[l-1]`.

[Tutorial on Prefix Sums](https://www.hackerrank.com/topics/prefix-sum)

[Video Tutorial](https://www.youtube.com/watch?v=pVS3yhlzrlQ)

[Peltorator on Prefix Sums](https://www.youtube.com/watch?v=5iW84xlL0j0): Great educational video, however it is in Russian with english subtitles.

-----
 
Here are some links to practice prefix sum based problems:

1. [Spoj CSUM](https://www.spoj.com/problems/CSUMQ/)
   
2. [Codechef Shivgod](https://www.codechef.com/problems/SHIVIGOD)
   
3. [Codeforces 433 B](https://codeforces.com/contest/433/problem/B)
   
4. [Codeforces 1118 B](https://codeforces.com/contest/1118/problem/B)

-----

Challenge Problems:

1. [Codeforces 1363 B](https://codeforces.com/contest/1363/problem/B)
