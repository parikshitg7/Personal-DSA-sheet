# 🚀 Data Structures & Algorithms: Patterns & Roadmap

A complete collection of LeetCode questions organized by **underlying logic** rather than random difficulty. Mastering these patterns allows you to solve 95% of interview questions.

---

<details>
<summary><h2>📚 ARRAYS & HASHING (Click to Expand)</h2></summary>

### **1. TWO POINTERS**
**Logic:** Use two indexes (usually `left` and `right`) moving towards each other or in parallel to find pairs or reverse logic.
* **When to use:** Sorted arrays, finding pairs/triplets, reversing, or "container" problems.

**🟢 ESSENTIALS (Covering Variations)**
- [167. Two Sum II - Input Array Is Sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/) *(Basic Convergence)*
- [15. 3Sum](https://leetcode.com/problems/3sum/) *(Fixed pointer + Two Pointers)*
- [11. Container With Most Water](https://leetcode.com/problems/container-with-most-water/) *(Greedy Width Shrinking)*

**🟡 PRACTICE**
- [977. Squares of a Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array/)
- [125. Valid Palindrome](https://leetcode.com/problems/valid-palindrome/)
- [16. 3Sum Closest](https://leetcode.com/problems/3sum-closest/)
- [42. Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/) *(Hard)*

<br>

### **2. SLIDING WINDOW**
**Logic:** Maintain a window (subarray) that grows or shrinks to satisfy a condition.
* **When to use:** "Longest/Shortest substring", "Max sum of size k", contiguous subarray problems.

**🟢 ESSENTIALS (Covering Variations)**
- [643. Maximum Average Subarray I](https://leetcode.com/problems/maximum-average-subarray-i/) *(Fixed Size Window)*
- [209. Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/) *(Dynamic Size - Shrinkable)*
- [3. Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) *(Dynamic Size + HashSet)*

**🟡 PRACTICE**
- [438. Find All Anagrams in a String](https://leetcode.com/problems/find-all-anagrams-in-a-string/)
- [567. Permutation in String](https://leetcode.com/problems/permutation-in-string/)
- [1004. Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii/)
- [424. Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement/)
- [76. Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/) *(Hard)*

<br>

### **3. PREFIX SUM (Range Queries)**
**Logic:** Pre-calculate sums so range `[i, j]` can be calculated in `O(1)`. Often combined with HashMaps for "Sum equals K".
* **When to use:** Range sum queries, "Subarray sum equals K".

**🟢 ESSENTIALS (Covering Variations)**
- [303. Range Sum Query - Immutable](https://leetcode.com/problems/range-sum-query-immutable/) *(Basic Definition)*
- [560. Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k/) *(HashMap Pattern - Very Important)*
- [238. Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/) *(Prefix + Suffix Logic)*

**🟡 PRACTICE**
- [724. Find Pivot Index](https://leetcode.com/problems/find-pivot-index/)
- [974. Subarray Sums Divisible by K](https://leetcode.com/problems/subarray-sums-divisible-by-k/)
- [525. Contiguous Array](https://leetcode.com/problems/contiguous-array/)

<br>

### **4. FAST & SLOW POINTERS (Cycle & In-Place)**
**Logic:** One pointer moves 1 step, another moves 2 steps. Also used for read/write pointers.
* **When to use:** Cycle detection, in-place removal, finding duplicates.

**🟢 ESSENTIALS (Covering Variations)**
- [283. Move Zeroes](https://leetcode.com/problems/move-zeroes/) *(Read/Write Pointers)*
- [287. Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/) *(Cycle Detection as Array)*

**🟡 PRACTICE**
- [26. Remove Duplicates from Sorted Array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/)
- [202. Happy Number](https://leetcode.com/problems/happy-number/)

<br>

### **5. INTERVALS (Merging & Overlapping)**
**Logic:** Dealing with time ranges. **Always sort by Start Time** first.
* **When to use:** "Merge", "Overlapping", "Schedule", "Meetings".

**🟢 ESSENTIALS (Covering Variations)**
- [56. Merge Intervals](https://leetcode.com/problems/merge-intervals/) *(Standard Merge Logic)*
- [57. Insert Interval](https://leetcode.com/problems/insert-interval/) *(Manual Traversal)*
- [435. Non-overlapping Intervals](https://leetcode.com/problems/non-overlapping-intervals/) *(Greedy Strategy)*

**🟡 PRACTICE**
- [452. Minimum Number of Arrows to Burst Balloons](https://leetcode.com/problems/minimum-number-of-arrows-to-burst-balloons/)
- [228. Summary Ranges](https://leetcode.com/problems/summary-ranges/)
- [986. Interval List Intersections](https://leetcode.com/problems/interval-list-intersections/)

<br>

### **6. CYCLIC SORT**
**Logic:** Iterate and swap `nums[i]` to `nums[nums[i] - 1]`.
* **When to use:** Array contains numbers in range `[1, N]` or `[0, N]`. Finds missing/duplicate numbers in O(N).

**🟢 ESSENTIALS (Covering Variations)**
- [268. Missing Number](https://leetcode.com/problems/missing-number/) *(Range 0 to N)*
- [442. Find All Duplicates in an Array](https://leetcode.com/problems/find-all-duplicates-in-an-array/) *(Finding Duplicates)*

**🟡 PRACTICE**
- [448. Find All Numbers Disappeared in an Array](https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/)
- [41. First Missing Positive](https://leetcode.com/problems/first-missing-positive/) *(Hard)*

<br>

### **7. MONOTONIC STACK**
**Logic:** Maintain a stack that is strictly increasing or decreasing.
* **When to use:** "Next Greater Element", "Next Smaller Element", Histogram areas.

**🟢 ESSENTIALS (Covering Variations)**
- [739. Daily Temperatures](https://leetcode.com/problems/daily-temperatures/) *(Next Greater Distance)*
- [496. Next Greater Element I](https://leetcode.com/problems/next-greater-element-i/) *(Basic)*

**🟡 PRACTICE**
- [503. Next Greater Element II](https://leetcode.com/problems/next-greater-element-ii/)
- [84. Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/) *(Hard)*

<br>

### **8. KADANE’S ALGORITHM**
**Logic:** Carry a local maximum; reset if the current sum becomes negative.
* **When to use:** "Maximum Contiguous Subarray Sum".

**🟢 ESSENTIALS**
- [53. Maximum Subarray](https://leetcode.com/problems/maximum-subarray/)
- [152. Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray/) *(Handling negatives)*

**🟡 PRACTICE**
- [918. Maximum Sum Circular Subarray](https://leetcode.com/problems/maximum-sum-circular-subarray/)

<br>

### **9. DUTCH NATIONAL FLAG (Partitioning)**
**Logic:** 3-way partitioning (Low, Mid, High pointers).
* **When to use:** Sorting 3 distinct elements (e.g., 0, 1, 2) in one pass.

**🟢 ESSENTIALS**
- [75. Sort Colors](https://leetcode.com/problems/sort-colors/)

<br>

### **10. 2D MATRIX SIMULATION**
**Logic:** Grid traversal logic.
* **When to use:** Rotating, spiraling, or mapping 2D arrays.

**🟢 ESSENTIALS**
- [48. Rotate Image](https://leetcode.com/problems/rotate-image/) *(Transpose + Reverse)*
- [54. Spiral Matrix](https://leetcode.com/problems/spiral-matrix/) *(Boundaries)*

**🟡 PRACTICE**
- [73. Set Matrix Zeroes](https://leetcode.com/problems/set-matrix-zeroes/)
- [59. Spiral Matrix II](https://leetcode.com/problems/spiral-matrix-ii/)

<br>

### **11. MOORE’S VOTING ALGORITHM**
**Logic:** Cancellation logic to find a majority element.
* **When to use:** Find element appearing `> N/2` or `> N/3` times in O(1) space.

**🟢 ESSENTIALS**
- [169. Majority Element](https://leetcode.com/problems/majority-element/)

**🟡 PRACTICE**
- [229. Majority Element II](https://leetcode.com/problems/majority-element-ii/)

</details>

---

<details>
<summary><h2>🔎 BINARY SEARCH (Click to Expand)</h2></summary>

### **1. BASIC & BOUNDARY**
**Logic:** Standard Binary search, but keep searching after finding target to find edges.
* **When to use:** Sorted array, search for index/element.

**🟢 ESSENTIALS**
- [704. Binary Search](https://leetcode.com/problems/binary-search/)
- [34. Find First and Last Position of Element in Sorted Array](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/)

**🟡 PRACTICE**
- [35. Search Insert Position](https://leetcode.com/problems/search-insert-position/)

<br>

### **2. SEARCH ON ANSWER (The "Koko" Pattern)**
**Logic:** The answer is a value in a range (e.g., 1 to 10^9). Binary search that value and check validity.
* **When to use:** "Minimum time to...", "Smallest divisor...", "Minimize max...".

**🟢 ESSENTIALS**
- [69. Sqrt(x)](https://leetcode.com/problems/sqrtx/) *(Math basic)*
- [875. Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/) *(Standard Min-Max)*
- [1011. Capacity To Ship Packages Within D Days](https://leetcode.com/problems/capacity-to-ship-packages-within-d-days/)

**🟡 PRACTICE**
- [410. Split Array Largest Sum](https://leetcode.com/problems/split-array-largest-sum/)

<br>

### **3. ROTATED SORTED ARRAY**
**Logic:** Identify which half is sorted, then check if target is in that half.
* **When to use:** "Search in rotated array", "Find min in rotated array".

**🟢 ESSENTIALS**
- [33. Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/)
- [153. Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/)

**🟡 PRACTICE**
- [81. Search in Rotated Sorted Array II](https://leetcode.com/problems/search-in-rotated-sorted-array-ii/)

<br>

### **4. PEAK FINDING**
**Logic:** Compare `mid` with neighbor `mid+1`.
* **When to use:** Bitonic array (mountain shape), find peak.

**🟢 ESSENTIALS**
- [162. Find Peak Element](https://leetcode.com/problems/find-peak-element/)

**🟡 PRACTICE**
- [852. Peak Index in a Mountain Array](https://leetcode.com/problems/peak-index-in-a-mountain-array/)

<br>

### **5. 2D BINARY SEARCH**
**Logic:** Map 2D indices to 1D (`row = mid/n`, `col = mid%n`) or start from top-right corner.

**🟢 ESSENTIALS**
- [74. Search a 2D Matrix](https://leetcode.com/problems/search-a-2d-matrix/)

**🟡 PRACTICE**
- [240. Search a 2D Matrix II](https://leetcode.com/problems/search-a-2d-matrix-ii/)

</details>
