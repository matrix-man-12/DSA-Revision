# C++ Essentials ONLY Repository

## Overview

This repository is dedicated to compiling a curated list of **less-used but essential C++ functions** and a **collection of important coding questions**. Whether you're a beginner looking to enhance your C++ skills or an experienced programmer wanting to refresh your knowledge, this repo aims to serve as a helpful resource.

## Features

- **Essential C++ Functions**: A comprehensive list of functions that may not be commonly used but are crucial for efficient coding.
- **Coding Questions**: A separate section containing important coding questions, each with a brief description and approach for solving them.

## Structure

- **C++ Functions**: Explore less-used functions that can improve your coding practices and efficiency.
- **Coding Questions**: Each question includes:
  - **Description**: A brief overview of the problem.
  - **Approach**: Suggested strategies for solving the problem.
  - **Link**: Direct links to the original questions for further practice.

### Table 1: Important Questions

| **#** | **Question**                                                            | **Description**                                                                                                                                                               | **Approach**                                                                                                                                                                   | **Data Structures**               | **Time Complexity (TC)** | **Space Complexity (SC)** |
|-------|-------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------|--------------------------|---------------------------|
| 1     | 238. [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/) | Given an integer array `nums`, return an array `output` such that `output[i]` is equal to the product of all the elements of `nums` except `nums[i]`.                    | 1. **Initialize** two arrays, `left` and `right`, of the same length as `nums`.  <br> 2. **Populate the `left` array**:  <br>   - `left[i]` contains the product of elements to the left of `i`.  <br> 3. **Populate the `right` array**:  <br>   - `right[i]` contains the product of elements to the right of `i`.  <br> 4. **Construct the `output` array**:  <br>   - `output[i]` is computed as `left[i] * right[i]`. | Array (for `left`, `right`, and `output`) | \(O(n)\)                  | \(O(n)\)                   |
| 2     | 271. [Encode and Decode Strings](https://leetcode.com/problems/encode-and-decode-strings/) | Design an algorithm to encode and decode strings. The encoding is done by length of each string followed by a special character and the string itself.                    | 1. **Encoding**: For each string, prepend its length and a special character (e.g., `#`) to it.  <br> 2. **Decoding**: Read the length of each string, extract the corresponding substring. | String manipulation                | \(O(n)\)                  | \(O(n)\)                   |

### Table 2: Important Functions

| **#** | **Function**   | **Parameters**                                                                 | **Returns**                  |
|-------|----------------|---------------------------------------------------------------------------------|------------------------------|
| 1     | `string.find()` | `const string& str` - substring to search <br> `size_t pos = 0` - start position (optional) | `size_t` - position of the first occurrence, or `npos` if not found |
| 2     | `atoi()`        | `const char* str` - C-string to convert                                          | `int` - the integer value     |
| 3     | `stoi()`        | `const string& str` - string to convert <br> `size_t* idx = 0` - pointer to store the index of the first invalid character (optional) | `int` - converted integer     |
| 4     | `to_string()`   | `T value` - value to convert to string                                          | `std::string` - string representation of the value |

## Contributing

Contributions are welcome! If you have suggestions for additional functions or questions to include, please feel free to open an issue or submit a pull request.
