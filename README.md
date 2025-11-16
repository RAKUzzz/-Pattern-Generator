# Number Pattern Generator

A simple Python function that generates a numeric pattern starting from `1` up to a specified integer `n`.  
This function includes basic input validation and returns the resulting pattern as a string.

---

## 📌 Function: `number_pattern(n)`

### ✔ Description
`number_pattern()` takes an integer `n`, validates the input, and returns a string containing a sequence of numbers from `1` to `n`, separated by spaces.

---

## 🔍 Features
- Validates that the input `n` is an integer  
- Checks that `n` is greater than 0  
- Automatically generates a sequence from `1` to `n`  
- Returns the result as a formatted string  
- Clear error messages for invalid inputs  

---

## 🧠 Function Logic

```python
def number_pattern(n):
    if not isinstance(n, int):
        return ('Argument must be an integer value.')
    if n < 1:
        return ('Argument must be an integer greater than 0.')
    n = n + 1
    number_list = []
    for num in range(1, n):
        number_list.append(num)
    result = ' '.join(str(m) for m in number_list)
    return str(result)

```

## 📝 Usage Examples
```python
print(number_pattern(5))

```
Output
```python
1 2 3 4 5

```

