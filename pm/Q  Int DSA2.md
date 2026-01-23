Todos
* check if we can borrow code samples from net or llm for 150 qs
* ask is to revise not to get depressed for poor coding capabilities
* correlate ask in q with the data set constraints and feasible solution

gh links
* https://github.com/ChunhThanhDe/Leetcode-Top-Interview


# Array / String
## merge sorted array
```python
def merge(nums1: list[int], m: int, nums2: list[int], n: int) -> None:
    """
    Do not return anything, modify nums1 in-place instead.
    
    Merges nums2 into nums1 in-place.
    nums1 has length m + n, where the last n elements are 0 and should be ignored
    initially.
    """
    
    # Initialize pointers for nums1 (actual elements), nums2, and the position 
    # to insert the next largest element in nums1.
    p1 = m - 1       # Pointer to the last element of the initial part of nums1
    p2 = n - 1       # Pointer to the last element of nums2
    p_insert = m + n - 1 # Pointer to the end of nums1 (the position to insert)

    # While there are elements in nums2 to be merged
    while p2 >= 0:
        # Check if p1 is still in bounds AND the element at p1 is greater
        # than the element at p2.
        if p1 >= 0 and nums1[p1] > nums2[p2]:
            # The larger element is in nums1
            nums1[p_insert] = nums1[p1]
            p1 -= 1 # Move p1 to the left
        else:
            # The larger element is in nums2 (or p1 is out of bounds, 
            # meaning all remaining elements are in nums2).
            nums1[p_insert] = nums2[p2]
            p2 -= 1 # Move p2 to the left
        
        # Move the insertion pointer to the left in every iteration
        p_insert -= 1

# Example Usage:
# nums1 = [1, 2, 3, 0, 0, 0], m = 3
# nums2 = [2, 5, 6], n = 3
# merge(nums1, m, nums2, n)
# print(nums1)  # Output: [1, 2, 2, 3, 5, 6]
```

## Remove Element
## Remove Duplicates from Sorted Array
## Remove Duplicates from Sorted Array II
## Majority Element
## Rotate Array
## Best Time to Buy and Sell Stock
## Best Time to Buy and Sell Stock II
## Jump Game
## Jump Game II
## H-Index
## Insert Delete GetRandom O(1)
## Product of Array Except Self
## Gas Station
## Candy
## Trapping Rain Water
## Roman to Integer
## Integer to Roman
## Length of Last Word
## Longest Common Prefix
```python
def longestCommonPrefix(strs: list[str]) -> str:
    """
    Finds the longest common prefix string amongst an array of strings.

    :param strs: A list of strings.
    :return: The longest common prefix, or an empty string "" if there is none.
    """
    if not strs:
        return ""

    # Take the first string as the initial reference/candidate prefix
    prefix = strs[0]

    # Iterate through the rest of the strings in the list
    for s in strs[1:]:
        # Continuously shorten the prefix from the end until it is
        # a prefix of the current string 's'
        while s.find(prefix) != 0:
            prefix = prefix[:-1]  # Shorten prefix by one character
            if not prefix:
                # If the prefix becomes empty, there's no common prefix
                return ""

    return prefix
```
## Reverse Words in a String
## Zigzag Conversion
## Find the Index of the First Occurrence in a String
## Text Justification

# Two Pointers

## Valid Palindrome

class Solution:
    def isPalindrome(self, s: str) -> bool:
        """
        Determines if a string is a valid palindrome by considering only
        alphanumeric characters and ignoring case.
        """
        # 1. Preprocessing: Filter and Normalize
        # Create a new string containing only lowercase alphanumeric characters.
        filtered_chars = "".join(char.lower() for char in s if char.isalnum())
        
        # 2. Check for Palindrome
        # A string is a palindrome if it reads the same forwards and backwards.
        # Python's slicing [::-1] creates the reversed string.
        return filtered_chars == filtered_chars[::-1]

# Example Usage:
# solution = Solution()
# print(solution.isPalindrome("A man, a plan, a canal: Panama"))  # Output: True
# print(solution.isPalindrome("race a car"))                      # Output: False
# print(solution.isPalindrome(" "))                               # Output: True

## Is Subsequence
## Two Sum II - Input Array Is Sorted
## Container With Most Water
## 3Sum

# Sliding Window
## Minimum Size Subarray Sum
## Longest Substring Without Repeating Characters
## Substring with Concatenation of All Words
## Minimum Window Substring

# Matrix
## Valid Sudoku
## Spiral Matrix
## Rotate Image
## Set Matrix Zeroes
## Game of Life

# Hashmap
## Ransom Note
## Isomorphic Strings
## Word Pattern
## Valid Anagram
## Group Anagrams
## Two Sum
## Happy Number
## Contains Duplicate II
## Longest Consecutive Sequence


# Intervals
## Summary Ranges
## Merge Intervals
## Insert Interval
## Minimum Number of Arrows to Burst Balloons


# Stack
## Valid Parentheses
## Simplify Path
## Min Stack
## Evaluate Reverse Polish Notation
## Basic Calculator


# Linked List
## Linked List Cycle
## Add Two Numbers
## Merge Two Sorted Lists
## Copy List with Random Pointer
## Reverse Linked List II
## Reverse Nodes in k-Group
## Remove Nth Node From End of List
## Remove Duplicates from Sorted List II
## Rotate List
## Partition List
## LRU Cache

# Binary Tree General
## Maximum Depth of Binary Tree
## Same Tree
## Invert Binary Tree
## Symmetric Tree
## Construct Binary Tree from Preorder and Inorder Traversal
## Construct Binary Tree from Inorder and Postorder Traversal
## Populating Next Right Pointers in Each Node II
## Flatten Binary Tree to Linked List
## Path Sum
## Sum Root to Leaf Numbers
## Binary Tree Maximum Path Sum
## Binary Search Tree Iterator
## Count Complete Tree Nodes
## Lowest Common Ancestor of a Binary Tree

# Binary Tree BFS
## Binary Tree Right Side View
## Average of Levels in Binary Tree
## Binary Tree Level Order Traversal
## Binary Tree Zigzag Level Order Traversal

# Binary Search Tree
## Minimum Absolute Difference in BST
## Kth Smallest Element in a BST
## Validate Binary Search Tree

# Graph General
## Number of Islands
## Surrounded Regions
## Clone Graph
## Evaluate Division
## Course Schedule
## Course Schedule II

# Graph BFS
## Snakes and Ladders
## Minimum Genetic Mutation
## Word Ladder


# Trie
## Implement Trie (Prefix Tree)
## Design Add and Search Words Data Structure
## Word Search II

# Backtracking
## Letter Combinations of a Phone Number
## Combinations
## Permutations
## Combination Sum
## N-Queens II
## Generate Parentheses
## Word Search

# Divide & Conquer
## Convert Sorted Array to Binary Search Tree
## Sort List
## Construct Quad Tree
## Merge k Sorted Lists

# Kadane's Algorithm
## Maximum Subarray
## Maximum Sum Circular Subarray

# Binary Search
## Search Insert Position
## Search a 2D Matrix
## Find Peak Element
## Search in Rotated Sorted Array
## Find First and Last Position of Element in Sorted Array
## Find Minimum in Rotated Sorted Array
## Median of Two Sorted Arrays

# Heap
## Kth Largest Element in an Array
## IPO
## Find K Pairs with Smallest Sums
## Find Median from Data Stream


# Bit Manipulation
## Add Binary
## Reverse Bits
## Number of 1 Bits
## Single Number
## Single Number II
## Bitwise AND of Numbers Range


# Math
## Palindrome Number
## Plus One
## Factorial Trailing Zeroes
## Sqrt(x)
## Pow(x, n)
## Max Points on a Line

# 1D DP
## Climbing Stairs
## House Robber
## Word Break
## Coin Change
## Longest Increasing Subsequence

# Multidimensional DP
## Triangle
## Minimum Path Sum
## Unique Paths II
## Longest Palindromic Substring
## Interleaving String
## Edit Distance
## Best Time to Buy and Sell Stock III
## Best Time to Buy and Sell Stock IV
## Maximal Square


## From Instagram
**Arrays**
* Find the missing number in an array of  to n
* Kadane's Algorithm (Maximum subarray sum)
* Find duplicate numbers in an array
* Merge two sorted arrays without extra space
* Rotate an array by K positions
* Find all pairs in an array that sum up to a given number
* Trapping Rain Water
* Find the longest consecutive subsequence
* Find the majority element
* Best time to buy and sell stock
* Merge intervals
* Next permutation of an array
* Find the minimum number of platforms required for a train station
* Maximum product subarray
* Find subarray with given sum
* Find median of two sorted arrays
* Rearrange array elements alternately (maximum, minimum)
* Find the largest element in an array

**Strings:**
* Check if two strings are anagrams
* Longest common prefix
* Check if a string is a palindrome
* Z-algorithm (Pattern matching)
* KMP Algorithm for pattern matching
* Longest palindromic substring
* Convert a string to an integer (lmplement atoi)
* Find the longest substring without repeating characters
* Rabin-Karp algorithm
* Roman to integer and vice versa
* group anagrams
* valid parentheses

**Stacks and Queues**
* Implement a stack using two queues
* Implement a queue using two stacks
* Next greater element
* Min stack (() space for minimum element)
* Valid parentheses (using stack)
* LRU Cache Implementation
* Sliding window maximum
* Circular tour (Petrol Pump problem)


**Linked Lists:**
*  Reverse a linked list
*  Detect a cycle in a linked list
*  Merge two sorted linked lists
*  Find the intersection point of two linked lists
*  Remove N-th node from the end of the list
*  Flatten a multilevel doubly linked list
*  Add two numbers represented by linked lists
*  Clone a linked list with random pointers
*  Palindrome linked list
*  Rotate a linked list

**Heaps**
* Kth largest element in an array
* Merge K sorted arrays
* Find the median from a data stream
* Top K frequent elements
* Minimum cost to connect all ropes
* Sort a nearly sorted array

**Trees:**
* Inorder,Preorder,Postordertraversalofabinarytree
* Levelordertraversalofabinarytree
* Findtheheightofabinarytree
* Checkifabinarytreeisbalanced
* Checkiftwotreesareidentical
* Lowestcommonancestorinabinarytree
* MaximumpathsumInabinarytree
* Diameterofabinarytree
* Checkifabinarytreeisabinarysearchtree
* Convertabinarytreetoadoublylinkedlist
* Zig-zagtraversalofabinarytree
* Kthsmallestlargestelementinabinarysearchtree
* Serializeanddeserializeabinarytree
* Flattenabinarytreetoalinkedlist

**Graphs:**
* Breadth-firstsearch(BFS)
* Depth-firstsearch(DFS)
* Detectacycleinanundirectedgraph
* Detectacycleinadirectedgraph
* Topologicalsort
* Dijkstra'salgorithm
* Bellman-Fordalgorithm
* Kruskal'salgorithm
* Prim'salgorithm
* FloydWarshallalgorithm
* Findwhetherapathexistsbetweentwonodes
* Countthenumberofislands

**DynamicProgramming:**
* Knapsackproblem
* Longestcommonsubsequence
* Longestincreasingsubsequence
* Editdistance
* Coinchangeproblem
* Wordbreakproblem
* Subsetsumproblem
* Maximumproductcutting
* Rodcuttingproblem
* Eggdroppingproblem
* Minimumsumpartition
* Palindromepartitioning

## Old Set of Qs from SME
**Strings**
- Find a maximum occurring character in the input string.
- Remove all duplicates from a given string.
- A program to check if strings are rotations of each other or not.
- Find the smallest window in a string containing all characters of another string
- Revere words in a given string.
- Find all distinct palindromic sub strings of a given string
- Remove all adjacent duplicate characters in a string
- Given a string, find the Run length encoding of given string.
- Check whether two strings are anagram of each other or not.
- Find the first non-repeating character from a stream of characters.
- Given an array of strings , find if the string can be of characters.
- Find a excel column name from a given column number.
- Convert one string to another using minimum number of given operation
- Check if a given sequence of moves for a robot is circular (or) not.
- Print concatenation of zig-zag string in 'n' rows.
- Minimum number of palindromic sub sequence to be removed to empty a binary string.
- All combinations of string that can be used to dial a number.

**Arrays**
- Find a pair in an array of size 'n', whose sum is X
- Find a majority element in an array of size 'n'
- Find the number occuring odd number of times in a given array of size 'n'
- Algorithm to reverse an array
- Algorithm to rotate array of size 'n' by 'd' elements
- Algorithm to segregate 0's and 1's in an array
- Find the maximum difference between two elements such that larger element appears after the smaller element
- Algorithm to merge an array of size 'n' into another array of size 'm+n'.
- Algorithm to find two repeating numbers in a given array
- Algorithm to find duplicate elements in O(n) time and O(1) extra space, for a given array of size 'n'
- Find the index in an array such that the sum of elements at lower indices is equal to the sum of elements at higher indices.
- Algorithm to find the maximum difference of j - i such that a[j] > a[i], for a given an array of 'n' elements.
- Algorithm to find the triplet whose sum is X
- Algorithm to find a sub array whose sum is X
- Algorithm to find the largest sub array with equal number of 0's and 1's
- Algorithm to find the number of triangles that can be formed with three different array elements as three sides of triangles, for a given unsorted array of n elements
- Algorithm to find the smallest integer value that can't be represented as sum of any subset of a given array.
- Algorithm to find the common element in given three sorted arrays
- Algorithm to find the contiguous sub-array with maximum sum, for a given array of postive and negative numbers.
- Given an array of integers, sort the array into a wave like array and return it. (arrange the element into a sequence such that a1>=a2<=a3>=a4<=a5----etc.
- Algorithm to find the next greater number formed after permuting the digits of given number
- Algorithm to find the sum of bit difference in all pairs that can be formed from array of n elements.
- Trapping rain water problem
- Algorithm to find the minimum number of platforms required for the railway station so that no train waits according to arrival and departure time
- Rotate 2-Dimentional array
- Lock and Key problem
- Rearrange an array so that a[i] becomes a[a[i]] with O(1) extra space
- Traverse a matrix of integers in spiral form
- Given an array consisting 0's, 1's and 2's, write a algorithm to sort it
- Given a positive number X, print all jumping numbers(all adjacent digits in it differ by 1) smaller than or equal to X
- Given an array and an integer 'k', find the maximum, for each and every contiguous subarray of size 'k'
- Search an element in a sorted rotated array
- Find the maximum value of a[j]-a[i]+a[l]-a[k], for every four indices i, j, k, l such that i< j < k < l. 

**Stack**
- Reversal of a stack
- Algorithm to find next greater element on the right side of an array.
- Implemention of the following operations in stack in O(1) time. Push(), pop(), isEmpty(), isFull() and getMin().
- Algorithm to find the celebrity in minimum number of questions in a party.
- Algorithm to the stock span problem is a financial problem where we have a series of 'n' daily price for a stock and we need to calculate span of stock’s price for all n days
- Algorithm to merge overlapping intervals
- Find the largest rectangular area possible in a given histogram.
- Given an integer array of size 'n', find the maximum of the minimum’s of every window size in the array.
- Calculate minimum number of bracket reversals needed to make an expression balenced.
- Design a stack, to find getmin() in O(1) time and O(1) space complexity.
- Find if an expression has duplicate or not....many more

**Queues**
- Given an array and an integer k, find the maximum for each and every contiguous subarray of size k.
- Implement LRU Cache.
- Find the first cicular tour that visits all petrol pumps
- Find the largest multiple of 3.


**Linked List**
- Algorithm to find the nth node from end of the linked list
- Algorithm to find the middle node in a linked list
- Algorithm to find the intersection point of two linked lists
- Reversal of linked list
- Algorithm to detect loop in linked list
- Algorithm to find starting node of a loop in a linked list
- Algorithm to check given linked list is palindrome (or) not
- Algorithm to reverse alternative K nodes in a single linked list
- Algorithm to clone a linked list with next and random pointer are given...many more


**Trees**
- Implement in order traversal without stack and recursion
- Convert a binary tree into its mirror tree
- Check if a given binary tree is sum tree or not
- Determine if the given two trees are identical or not
- Print out all of its roof to leaf paths in a given binary tree
- Find a lowest common ancestor of a given two nodes in a abinary search tree
- Find a lowest common ancestor of a given two nodes in a binary tree
- Level order traversal in spiral form
- Convert an arbitrary binary tree to a tree that holds children sum property
- Find the Diameter of a BST
- Construct tree from given inorder and post order traversal
- Convert a Binary Tree to a circular DLL
- Evaluation of expression tree
- Print extreme node of each level of Binary Tree in alternative order
- Print cousins of a given node in Binary Tree
- Diagonal traversal of Binary Tree
- Construct tree from ancestor matrix
- Given a Binary Tree, find vertical sum of the nodes that are in same vertical line.
- Find multiplication of sums of data of leaves at same level.
- Given a binary tree, find maximum value we can get by subtracting value of node B from value of node A
- Print nodes in a top view of Binary Tree.
- Given a Binary Tree and a number k, remove all nodes that lie only on root to leaf path(s) of length smaller than k.
- Serialize and deserialize an N-ary tree.
- Reverse alternate levels of a perfect Binary Tree.
- Print all nodes that are at distance k from a leaf node.
- Custom tree problem.
- Construct complete binary tree from its linked list representation.
- Find next right nodes of given leafs in a binary tree.
- Given a binary tree, print boundary nodes of the binary tree Anti-Clockwise starting from the root.
- Convert a given tree to its sum tree.
- Given a binary tree, find out if the tree can be folded or not.
- Find largest sub tree having identical left and right sub tree.
- Convert a normal binary search tree to balanced BST.
- Check if removing an edge can divide a binary tree in the form of n-ary tree.
- locking and unlocking of resource arranged on the form of n-ary tree.

**Heaps**
- Find K largest (or smallest) elements in array.
- Tournament tree method using binary heap .
- Find a Median in a stream of integers.
- Sort a nearly sorted array(or k sorted).
- Given array representation of min Heap, convert it to max Heap.
- Check if a given binary tree is Heap.
- Find kth largest element in a stream.
- Print all elements in sorted order from row and column wise sorted matrix.
- Given n ropes of different length, connect with minimum cost.
- Given k sorted arrays of size n each, merge them.
- Design an efficient data structure for given operations find min(), findmax(), deletemin(), Insert(),delete().

**Graphs**
- Given a directed graph G=(V,E), find whether G has a cycle.
- Given a directed graph G=(V,E), find whether there is path between two vertices vi and vj.
- Given a 2D boolean matrix, find the number of islands.
- Given an undirected graph G=(V,E), find whether G has a cycle or not. (Union-Find Algorithm).
- Given a connected undirected graph, find all the articulation points.
- Given an undirected graph, find all the bridges in the graph.
- Given a directed graph, find all the strongly connected components.
- Given a weighted directed acyclic graph, find the shortest path from a vertex to all the other vertices.
- Given a weighted directed acyclic graph, find the longest path from a vertex to all the other vertices.
- Check whether a given graph is bipartite or not.
- Find number of connections a person till nth level.
- Bit Manipulation
- Mathematical Algorithms

**Divide & Conquer**
- Find the median of two sorted arrays
- Count inversions in an array
- Find majority Element in a sorted array
- Find the maximum and minimum of an array using minimum number of comparisons
- The skyline problem
- Given two binary strings that represent value of two integers, find the product of two strings.
- Given an array of integers. Find a peak element in it.
- Find the missing number in Arithmetic Progression
- Given an array of n points in the plane, find out the closest pair of points in the array.

**Pattern searching**
- Given a text and a pattern, find all occurrences of pattern in a given text. Using naive approach.
- Given a text and a pattern, find all occurrences of pattern in a given text. Using Rabin-Karp algorithm.
- Given a text and a pattern, find all occurrences of pattern in a given text. Using Finite automata approach.
- Given a text and a pattern, find all occurrences of pattern in a given text. Using Boyer moore algorithm.
- Given a text and a pattern, find all occurrences of pattern in a given text. Using KMP algorithm.
- Given a string, find the longest sub string which is palindrome using manacher’s algorithm
- Find all occurrences of a given word in a matrix.

**Back Tracking**
- Print all permutations of a given string.
- Find subset of elements that are selected from a given set whose sum adds up to a given number K.
- Given a set of n integers, divide the set in two subsets of n/2 sizes each such that the difference of the sum of two subsets is as minimum as possible.
- Solve Sudoku using backtracking.
- Given a maze, NxN matrix. A rat has to find a path from source to destination. Left top corner is the source and right bottom corner is destination. There are few cells which are blocked, means rat can¬not enter into those cells.


**Greedy Algorithms**
- Given an array of jobs with different time intervals. Find the minimum time to finish all jobs.
- Given a universe of n elements, collection of subsets. Find a minimum cost sub collection that covers all elements.
- Given n cities and distances between every pair of cities, select k cities to place warehouses, such that the maximum distance of a city to a warehouse is minimized.

**Dynamic Programming**
- Find the length of the longest sub sequence of a given sequence such that all elements of the sub sequence are sorted in increasing order.
- Given two sequences, find the length of longest sub sequence present in both of them.
- Given a cost matrix and a position (m, n) , Find cost of minimum cost path to reach (m, n) from (0, 0).
- Coin change problem.
- Find the length of the longest palindrome sub sequence.
- Find th sum of maximum sum sub sequence of the given array.
- You have a rectangular grid of dimension 2 x n. You need to find out the maximum sum such that no two chosen numbers are adjacent , vertically, diagonally (or) horizontally.
- Given an array A with n elements and array B with m elements. With m you have to insert (n-m) zero's in between array B such that the dot product of array A and array B is maximum.
- Transform a string into palindrome on removing at most k characters from it.
- Find the longest even length sub string such that sum of first and second half is same..
- Count number of ways to reach a given score in a game.
- Compute sum of digits in all number from 1 to n.
- Collect maximum points in a grid using two traversals
- Given a 2xn board and titles of size 2x1, count the number of ways to tile he given board using the 2x1 tiles..
- Count the number of ways we can parenthesize the expression so that the value of expression evaluates to true.
- Given a Binary Tree, find size of the Largest Independent Set(LIS) in it.
- There are n stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs at a time. Count the number of ways, the person can reach the top.
- Find total number of non-decreasing numbers with n digits.
- Egg dropping problem.
- Given a rod of length n inches and an array of prices that contains prices of all pieces of size smaller than n. Determine the maximum value obtainable by cutting up the rod and selling the pieces.
- Given N jobs where every job is represented by Start Time, Finish Time, Profit or Value Associated. Find the maximum profit subset of jobs such that no two jobs in the subset overlap.
- Box stacking problem.
- Given an input string and a dictionary of words, find out if the input string can be segmented into a space-separated sequence of dictionary words.
- Given a binary matrix, find out the maximum size square sub-matrix with all 1s.
- Find the maximum coins you can collect by bursting the balloons wisely.










