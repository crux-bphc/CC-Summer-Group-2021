(Optional) Part 1 Episode 1.5/4: C++ STL Extra Resources
=====

The C++ STL can be broadly divided into four parts:

1. Containers
2. Functor (Not important)
3. Iterators
4. Algorithms

Containers
-----

Containers are used to manage collections of objects of a certain kind. There are several different types of containers like dequeue, list, vector, map etc.

A short overview of all containers:

1. [Vector](https://en.cppreference.com/w/cpp/container/vector) - Dynamic arrays


2. [String](https://en.cppreference.com/w/cpp/string/basic_string) - Essentially a vector of characters with extra string functionality.


3. [List](https://en.cppreference.com/w/cpp/container/list) - Doubly linked lists


4. [Dequeue](https://en.cppreference.com/w/cpp/container/deque) - Double ended Queue


5. [Array](https://en.cppreference.com/w/cpp/container/array) - A container that encapsulates fixed size arrays.


6. [Queue](https://en.cppreference.com/w/cpp/container/queue) - Queue data structure


7. [Stack](https://en.cppreference.com/w/cpp/container/stack) - Stack Data structure


8. [Priority Queue](https://en.cppreference.com/w/cpp/container/priority_queue) - A priority queue is a container adaptor that provides constant time lookup of the largest (by default) element, at the expense of logarithmic insertion and extraction.


9.  [Set](https://en.cppreference.com/w/cpp/container/set) - It is an associative container that contains a sorted set of unique objects.


10. [Multiset](https://en.cppreference.com/w/cpp/container/multiset) - Same as set but supports repeated elements


11. [Map](https://en.cppreference.com/w/cpp/container/map) - It is a sorted associative container that contains key-value pairs with unique keys. 


12. [Multimap](https://en.cppreference.com/w/cpp/container/multimap) - Same as map, while permitting multiple entries with the same key.


13. [Unordered_set](https://en.cppreference.com/w/cpp/container/unordered_set) - It is an associative container that contains a set of unique objects of type Key. Search, insertion, and removal have average constant-time complexity.


14. [Unordered_multiset](https://en.cppreference.com/w/cpp/container/unordered_multiset) - Same as unordered set but supports repeated elements.


15. [Unordered_map](https://en.cppreference.com/w/cpp/container/unordered_map) - It is an associative container that contains key-value pairs with unique keys. Search, insertion, and removal of elements have average constant-time complexity.


16. [Unordered_multimap](https://en.cppreference.com/w/cpp/container/unordered_multimap) - Same as map but supports mapping one key to many values.

It is recommended that you go through the methods present on each of these containers and understand what they achieve and the time complexity of that method.

-----

Extra: Range Based For Loops
-----

A wonderful feature that was introduced in recent versions of C++ is the **range based for loop.**

For those that come from other programming backgrounds, this would be a metaphor to a For-Each loop.

A range based for loop provides an easy way of iterating over complex containers without having to setup your beginning and ending conditions.

[Tutorial on range based for loops](https://www.programiz.com/cpp-programming/ranged-for-loop)

[Video Tutorial](https://www.youtube.com/watch?v=8qrZYjL2jBg)

-----

Iterators
-----

**PS:** [ Iterators are not all that common but sometimes you'll have no choice but to use them and that's why this section exists. *Example* - Deleting a single element from a multiset can be achieved using mostly iterators. ]

An iterator is an object (like a pointer) that points to an element inside the container. We can use iterators to move through the contents of the container. They can be visualized as something similar to a pointer pointing to some location and we can access the content at that particular location using them.

[Tutorial on Iterators](https://www.simplilearn.com/tutorials/cpp-tutorial/iterators-in-cpp)

[Video Tutorial](https://www.youtube.com/watch?v=SgcHcbQ0RCQ)

-----

Algorithms
-----

The C++ STL comes with some pre-implemented algorithms and it is important for you to at least know that the following ones exist at your disposal:

1. [std::sort](https://en.cppreference.com/w/cpp/algorithm/sort) - Sorting a container.
   
2. [std::reverse](https://en.cppreference.com/w/cpp/algorithm/reverse) - Reversing a container.
   
3. [std::max_element](https://en.cppreference.com/w/cpp/algorithm/max_element) - Returns an iterator to the largest element of a container.
   
4. [std::min_element](https://en.cppreference.com/w/cpp/algorithm/min_element) - Returns an iterator to the smallest element of a container.
   
5. [std::binary_search](https://en.cppreference.com/w/cpp/algorithm/binary_search) - Binary search in an ordered container to check existence of element.
   
6. [std::lower_bound](https://en.cppreference.com/w/cpp/algorithm/lower_bound) - Returns an iterator pointing to the first element in the range that is not less than (i.e. greater or equal to) value.
   
7. [std::upper_bound](https://en.cppreference.com/w/cpp/algorithm/upper_bound) - Returns an iterator pointing to the first element in the range that is greater than value.
   
8.  [std::next_permutation](https://en.cppreference.com/w/cpp/algorithm/next_permutation) - Permutes the range into the next permutation, where the set of all permutations is ordered lexicographically with respect to operator < or comp.

9.  [std::prev_permutation](https://en.cppreference.com/w/cpp/algorithm/prev_permutation) - Transforms the range into the previous permutation from the set of all permutations that are lexicographically ordered with respect to operator < or comp.

[Video Tutorial on Lower and Upper bound](https://www.youtube.com/watch?v=Cg7SI0WtmXY)
