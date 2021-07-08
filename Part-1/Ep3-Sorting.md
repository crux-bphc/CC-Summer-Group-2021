Part 1 Episode 3/4: Sorting
=====

Simply put, sorting is the procedure of re-ordering a list of **n** elements A1,A2,A3....An based on a pre-defined comparison operator (a comparator), such that the final ordering satisfies the following criteria:

A1 <= A2 <= A3 .... <= An

(This is assuming you wished for the final ordering to be in an ascending or increasing order)

A decreasing order would look like:

A1 >= A2 >= A3 .... >= An

If you ever see the word **strict** ordering or **strictly** increasing or **strictly** decreasing, it means that the ordering is no longer a **weak ordering** and instead is now either of the form:

1. A1 < A2 < A3 .... < An

2. A1 > A2 > A3 .... > An

-----

There are several algorithms out there that take care of sorting for you:

1. Bubble Sort: O(n^2)
2. Selection Sort: O(n^2)
3. Insertion Sort: O(n^2)
4. Quick Sort: O(n^2)
5. Heap Sort: O(n log(n))
6. Merge Sort: O(n log(n))

Most common sorting algorithms use the [Merge Sort](https://medium.com/karuna-sehgal/a-simplified-explanation-of-merge-sort-77089fe03bb2) as the core of their logic, some others use a hybrid between multiple of the above listed algorithms.

An [optional read](https://theartofmachinery.com/2019/01/05/sorting_is_nlogn.html) on why the best asymptotic time complexity for sorting algorithms is O(n log(n)).

-----

**Important**: Always prefer to use predefined built-in sorting algorithms because there exist highly optimized and trusted implementations provided by most languages. Always try to use those before turning to user defined functions.

For example, in C++, the `<algorithm>` header file contains an implementation of a sorting algorithm that can be called within your program as `std::sort`. Read more about [std::sort here](https://en.cppreference.com/w/cpp/algorithm/sort).

-----

Custom Sort Operator | Comparator
-----

Sometimes the question requires you to sort a collection of items based on a non-standard compare operation between them.

For example, let's say you want to sort a list of strings first by their length and only then by their alphabetical order.

In such cases, you are required to write a custom compare operator (a comparator) and pass that to your sorting function.

Thus, in the example above, you would define your comparator as:

```C++
bool comp(const string &s1, const string &s2) {
    if(s1.size() < s1.size()) {
        return true; // return true if you want s1 to appear before s2 in the sorted order
    }
    else if(s2.size() < s1.size()) {
        return false; // return false if you want s2 to appear before s1 in the sorted order
    }
    else {
        return s1 < s2; // fallback to normal lexicographical comparison
    }
}

```

You can then pass this custom comparator to the `std::sort` function. Check `std::sort` [documentation](https://en.cppreference.com/w/cpp/algorithm/sort). for more examples.

[Video Tutorial on C++ Custom Comparators](https://www.youtube.com/watch?v=3pvZhwp0U9w)

-----

**Interesting:** While I did mention above that we certainly cannot achieve sorting faster than O(n log(n)), there are special situations in which we can use an algorithm that sorts a set of items in faster than O(n log(n)) time:

1. [Counting Sort](https://www.geeksforgeeks.org/counting-sort/): It is a sorting technique based on keys between a specific range. It works by counting the number of objects having distinct key values (kind of hashing). Then doing some arithmetic to calculate the position of each object in the output sequence.
2. Bucket Sort (Not very important)
3. Radix Sort (Not very important)

-----

Here are some practice problems on sorting:

1. [Codeforces 1399 A](https://codeforces.com/problemset/problem/1399/A)
2. [Codeforces 1092 B](https://codeforces.com/problemset/problem/1092/B)
3. [Codeforces 984 A](https://codeforces.com/problemset/problem/984/A)
4. [Codeforces 339 A](https://codeforces.com/problemset/problem/339/A)

**Challenge Problems:**

1. [Codeforces 977 C](https://codeforces.com/problemset/problem/977/C)
2. [Codeforces 1174 B](https://codeforces.com/problemset/problem/1174/B)
