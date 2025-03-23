# helper functions 

# header1

```python
def print_header1(text):
    text = text.upper() 
    box_length = len(text) + 2
    print("\n" + "+" + "-" * box_length + "+")
    print(f"| {text} |") 
    print("+" + "-" * box_length + "+")
```

# header2

```python
def print_header2(text):
    text = text.upper()
    print(f"\n[ {text} ]") 
```

# message

```python
def print_message(message, depth=0):
    indent = ' ' * depth
    print(f"{indent}-> {message}")
```
