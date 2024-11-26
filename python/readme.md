### Python Interview Questions.
# Python Interview Questions

## 1. What are Python decorators and how do they work?
Decorators are functions that modify the functionality of another function. They allow you to wrap another function to extend its behavior without permanently modifying it.

### Example:
```python
def decorator_function(original_function):
    def wrapper_function():
        print("Wrapper executed before {}".format(original_function.__name__))
        return original_function()
    return wrapper_function

@decorator_function
def display():
    return "Display function executed"

print(display())