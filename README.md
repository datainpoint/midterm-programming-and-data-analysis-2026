# midterm-programming-and-data-analysis-2026

> Midterm: Programming and Data Analysis 2026.

- Define specified functions in `answers.py`.
- Run `test-runner.py` to validate your answers.
- Upload your `answers.py` to NTU COOL before deadline.
- Do not use `input()` functions in `answers.py`, it breaks batch grading.
- Do not include `test-runner.py` in `answers.py`, only submit functions defined by you.

## 01. Define a function `format_date_with_padding_zero()` which formats month and day with padding zero.

```python
def format_date_with_padding_zero(yyyy: int, mm: int, dd: int) -> str:
    """
    >>> format_date_with_padding_zero(2023, 9, 9)
    '2023-09-09'
    >>> format_date_with_padding_zero(2023, 9, 10)
    '2023-09-10'
    >>> format_date_with_padding_zero(2023, 10, 9)
    '2023-10-09'
    >>> format_date_with_padding_zero(2023, 10, 10)
    '2023-10-10'
    >>> format_date_with_padding_zero(2024, 1, 1)
    '2024-01-01'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a function `convert_iso_8601_date_to_mandarin()` which converts a ISO-8601 date string to mandarin.

```python
def convert_iso_8601_date_to_mandarin(iso_8601_date: str) -> str:
    """
    >>> convert_iso_8601_date_to_mandarin("2026-10-31")
    '二零二六年十月三十一日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-30")
    '二零二六年十月三十日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-27")
    '二零二六年十月二十七日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-25")
    '二零二六年十月二十五日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-20")
    '二零二六年十月二十日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-19")
    '二零二六年十月十九日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-10")
    '二零二六年十月十日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-09")
    '二零二六年十月九日'
    >>> convert_iso_8601_date_to_mandarin("2026-10-01")
    '二零二六年十月一日'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a function `format_ntd_with_dollar_sign_commas_and_decimals()` which formats integer with dollar sign and commas.

```python
def format_ntd_with_dollar_sign_commas_and_decimals(ntd: int) -> str:
    """
    >>> format_ntd_with_dollar_sign_commas_and_decimals(1000)
    '$1,000.00 NTD'
    >>> format_ntd_with_dollar_sign_commas_and_decimals(1000000)
    '$1,000,000.00 NTD'
    >>> format_ntd_with_dollar_sign_commas_and_decimals(1000000000)
    '$1,000,000,000.00 NTD'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a function `semantic_typing()` which returns the type of input semantically.

```python
def semantic_typing(x) -> str:
    """
    >>> semantic_typing(5566)
    'The type of your input 5566 is an integer.'
    >>> semantic_typing(3.1415)
    'The type of your input 3.1415 is a float.'
    >>> semantic_typing(False)
    'The type of your input False is a boolean.'
    >>> semantic_typing(True)
    'The type of your input True is a boolean.'
    >>> semantic_typing("Python")
    'The type of your input Python is a string.'
    >>> semantic_typing(None)
    'The type of your input None is a NoneType.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a function `semantic_calculator()` which operates a few simple numeric calculations.

```python
def semantic_calculator(x: int, y: int, operator: str):
    """
    >>> semantic_calculator(55, 66, "+")
    121
    >>> semantic_calculator(55, 66, "-")
    -11
    >>> semantic_calculator(3, 5, "*")
    15
    >>> semantic_calculator(3, 5, "/")
    0.6
    >>> semantic_calculator(3, 5, "//")
    0
    >>> semantic_calculator(3, 5, "**")
    243
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a function `is_palindrome()` which returns `False` if input string is not a palindrome word, otherwise returns `True`.

Source: <https://en.wikipedia.org/wiki/Palindrome>

```python
def is_palindrome(x: str) -> bool:
    """
    >>> is_palindrome("yay")
    True
    >>> is_palindrome("radar")
    True
    >>> is_palindrome("level")
    True
    >>> is_palindrome("python")
    False
    >>> is_palindrome("data")
    False
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a function `square_negatives()` which returns positive args given `*args`.

```python
def square_negatives(*args) -> list:
    """
    >>> square_negatives(-3, -2, -1, 0, 1, 2, 3)
    [9, 4, 1]
    >>> square_negatives(-3, -2, -1, 0, 1, 2, 3, '4', '5')
    [9, 4, 1]
    >>> square_negatives(-3, -2, -1, False, True, 2, 3, '4', '5')
    [9, 4, 1]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `remove_duplicates_and_sort()` which removes duplicate elements for `*args` then sort with ascending order.

```python
def remove_duplicates_and_sort(*args) -> list:
    """
    >>> remove_duplicates_and_sort(2, 3, 5, 7, 11, 11, 7, 5, 3, 2)
    [2, 3, 5, 7, 11]
    >>> remove_duplicates_and_sort(13, 17, 19, 23, 29, 31, 31, 29, 23, 19, 17, 13)
    [13, 17, 19, 23, 29, 31]
    >>> remove_duplicates_and_sort(10, 9, 8, 6, 4, 1, 1, 4, 6, 8, 9, 10)
    [1, 4, 6, 8, 9, 10]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `reverse_key_value_pairs()` which reverses key and value pairs given `**kwargs`.

```python
def reverse_key_value_pairs(**kwargs):
    """
    >>> reverse_key_value_pairs(twn="tw")
    {'tw': 'twn'}
    >>> reverse_key_value_pairs(twn="tw", jpn="jp")
    {'tw': 'twn', 'jp': 'jpn'}
    >>> reverse_key_value_pairs(twn="tw", jpn="jp", usa="us")
    {'tw': 'twn', 'jp': 'jpn', 'us': 'usa'}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `is_prime()` which returns `False` if input integer is not a prime number, otherwise returns `True`.

Source: <https://en.wikipedia.org/wiki/Prime_number>

```python
def is_prime(x: int):
    """
    >>> is_prime(1)
    False
    >>> is_prime(2)
    True
    >>> is_prime(3)
    True
    >>> is_prime(4)
    False
    >>> is_prime(5)
    True
    """
    ### BEGIN SOLUTION

    ### END SOLUTION
```

## 11. Define a function `range_primes()` which returns a range of primes given start(inclusive) and stop(exclusive).

```python
def range_primes(start: int, stop: int):
    """
    >>> range_primes(0, 5)
    [2, 3]
    >>> range_primes(6, 15)
    [7, 11, 13]
    >>> range_primes(17, 30)
    [17, 19, 23, 29]
    >>> range_primes(31, 37)
    31
    >>> range_primes(35, 37)
    None
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 12. Define a function `range_fizz_buzz()` which returns a range of fizz-buzz numbers/strings given start(inclusive) and stop(exclusive).

Source: <https://en.wikipedia.org/wiki/Fizz_buzz>

```python
def range_fizz_buzz(start: int, stop: int) -> list:
    """
    >>> range_fizz_buzz(1, 6)
    [1, 2, 'Fizz', 4, 'Buzz']
    >>> range_fizz_buzz(6, 11)
    ['Fizz', 7, 8, 'Fizz', 'Buzz']
    >>> range_fizz_buzz(11, 16)
    [11, 'Fizz', 13, 14, 'Fizz Buzz']
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 13. Define a function `find_idxmin_idxmax()` which finds the indices of minimum and maximum values, respectively given a `list`.

```python
def find_idxmin_idxmax(x: list) -> dict:
    """
    >>> find_idxmin_idxmax([2, 3, 5, 7, 11])
    {'idxmin': [0], 'idxmax': [4]}
    >>> find_idxmin_idxmax([2, 3, 5, 7, 11, 11, 7, 5, 3, 2])
    {'idxmin': [0, 9], 'idxmax': [4, 5]}
    >>> find_idxmin_idxmax([10, 9, 8, 6, 4, 1])
    {'idxmin': [5], 'idxmax': [0]}
    >>> find_idxmin_idxmax([10, 9, 8, 6, 4, 1, 1, 4, 6, 8, 9, 10])
    {'idxmin': [5, 6], 'idxmax': [0, 11]}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 14. Define a function `pig_latin()` which plays the Pig Latin language game with function inputs.

- For words that begin with consonant sounds, all letters before the initial vowel are placed at the end of the word sequence. Then, "ay" is added. e.g. "pig" -> "igpay". When words begin with consonant clusters (multiple consonants that form one sound), the whole sound is added to the end. e.g. "smile" -> "ilesmay"
- For words that begin with vowel sounds, the vowel is left alone, and "yay" is added to the end. e.g. "eat" -> "eatyay"

Source: <https://en.wikipedia.org/wiki/Pig_Latin>

```python
def pig_latin(x: str) -> str:
    """
    >>> pig_latin("pig")
    'igpay'
    >>> pig_latin("smile")
    'ilesmay'
    >>> pig_latin("eat")
    'eatyay'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 15. Define a function `fibonacci()` which returns the famous Fibonacci sequence in a `list` given `a`, `b` ($a \le b$) and `length` as parameters.

Source: <https://en.wikipedia.org/wiki/Fibonacci_sequence>

```python
def fibonacci(a: int, b: int, length: int) -> list:
    """
    >>> fibonacci(0, 1, 5)
    [0, 1, 1, 2, 3]
    >>> fibonacci(0, 1, 7)
    [0, 1, 1, 2, 3, 5, 8]
    >>> fibonacci(0, 1, 11)
    [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```