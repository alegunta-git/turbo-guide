Todos
* check if we can borrow code samples from net or llm for 150 qs
* ask is to revise not to get depressed for poor coding capabilities
* correlate ask in q with the data set constraints and feasible solution

gh links
* https://github.com/ChunhThanhDe/Leetcode-Top-Interview

## Leetcode Patterns
* 0/1 Knapsack (DP)
* Backtracking ,  
* Bitwise XOR 
* Cyclic Sort
* Divide and Conquer
* Dynamic Programming
* Fast & Slow Pointers , 
* Greedy
* In-place Reversal LL 
* Island (Matrix Traversal) ,
* K-way Merge
* Merge Intervals , 
* Modified Binary Search 
* Monotonic Stack ,
* Prefix Sum
* Recursion
* Sliding Window
* Subsets , 
* Top 'K' Elements , 
* Topological Sort ,  
* Tree Breadth First Search , 
* Tree Depth First Search 
* Trie 
* Two Heaps , 
* Two Pointers ,


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

