# C++ Essentials ONLY Repository

## What's here

This repository is dedicated to compiling a curated list of **Important coding questions** and **less-used but essential C++ functions**. 

### Table 1: Important Questions

| **#** | **Question**                                                            | **Description**                                                                                                                                                               | **Approach**                                                                                                                                                                   | **Data Structures**               | **Time Complexity (TC)** | **Space Complexity (SC)** |
|-------|-------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------|--------------------------|---------------------------|
| 1     | 238. [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/) | Given an integer array `nums`, return an array `output` such that `output[i]` is equal to the product of all the elements of `nums` except `nums[i]`.                    | 1. **Initialize** two arrays, `left` and `right`, of the same length as `nums`.  <br> 2. **Populate the `left` array**:  <br>   - `left[i]` contains the product of elements to the left of `i`.  <br> 3. **Populate the `right` array**:  <br>   - `right[i]` contains the product of elements to the right of `i`.  <br> 4. **Construct the `output` array**:  <br>   - `output[i]` is computed as `left[i] * right[i]`. | Array (for `left`, `right`, and `output`) | \(O(n)\)                  | \(O(n)\)                   |
| 2     | 271. [Encode and Decode Strings](https://leetcode.com/problems/encode-and-decode-strings/) | Design an algorithm to encode and decode strings. The encoding is done by length of each string followed by a special character and the string itself.                    | 1. **Encoding**: For each string, prepend its length and a special character (e.g., `#`) to it.  <br> 2. **Decoding**: Read the length of each string, extract the corresponding substring. | String manipulation                | \(O(n)\)                  | \(O(n)\)                   |
| 3     | 128. [Longest Consecutive Sequence](https://leetcode.com/problems/longest-consecutive-sequence/) | Given an unsorted array of integers `nums`, return the length of the longest consecutive elements sequence.                                                                 | 1. **Insert** all numbers into an unordered set.  <br> 2. **For each element** `num` in the set, check if `num-1` is not in the set, which means `num` is the start of a sequence.  <br> 3. **Count** the length of the sequence starting from `num` by checking consecutive elements.  <br> 4. **Update** the maximum sequence length accordingly. | HashSet                          | \(O(n)\)                  | \(O(n)\)                   |

*** 

### Table 2: Important Functions

| **#** | **Function**   | **Parameters**                                                                 | **Returns**                  |
|-------|----------------|---------------------------------------------------------------------------------|------------------------------|
| 1     | `string.find()` | `const string& str` - substring to search <br> `size_t pos = 0` - start position (optional) | `size_t` - position of the first occurrence, or `npos` if not found |
| 2     | `atoi()`        | `const char* str` - C-string to convert                                          | `int` - the integer value     |
| 3     | `stoi()`        | `const string& str` - string to convert <br> `size_t* idx = 0` - pointer to store the index of the first invalid character (optional) | `int` - converted integer     |
| 4     | `to_string()`   | `T value` - value to convert to string                                          | `std::string` - string representation of the value |

## About Contributions

Contributions are welcome! If you have suggestions for additional functions or questions to include, please feel free to open an issue or submit a pull request.
