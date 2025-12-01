## Overview
This notebook explains lambda functions in Python and demonstrates how they can be used to build short, anonymous functions without the need for the `def` keyword. Lambda expressions allow cleaner one-liner logic suited for quick evaluations and functional programming use cases.

## Notebook Contents
- What lambda functions are
- Syntax and structure
- Single and multi-parameter lambda expressions
- Usage with map filter reduce
- Lambda as sorting keys
- Difference from normal functions
- Practice examples and reference notes

## Key Concepts
- **Lambda functions are anonymous one-line functions in Python**
- **It must contain only one expression which returns a value**
- **Lambdas can accept multiple parameters**
- Commonly used with higher-order functions like `map()` `filter()` `reduce()`
- Perfect for temporary operations that do not require naming a function
- Ideal in functional-style programming where short transformations are needed

### Lambda Function Syntax
```python
lambda arguments: expression


## Code
Code Examples Covered
# 1. Lambda for cube
cube = lambda x: x*x*x
print(cube(3))

# 2. Lambda for sum of two numbers
sum_two = lambda a, b: a + b
print(sum_two(5, 10))

# 3. Lambda inside map()
nums = [1,2,3,4]
squared = list(map(lambda x: x*x, nums))
print(squared)

# 4. Lambda as filter condition
even_nums = list(filter(lambda x: x%2==0, nums))
print(even_nums)

# 5. Lambda for sorting key
items = [(3,'c'),(1,'a'),(2,'b')]
sorted_list = sorted(items, key=lambda x:x[0])
print(sorted_list)
