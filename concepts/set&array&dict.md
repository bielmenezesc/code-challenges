# Sets

É uma lista não ordenada que só vai conter **elementos únicos**.

```python
# Create a set
my_set = set()

# Add an element to the set
my_set.add(5)
my_set.add(4)

# Remove an element from the set
my_set.remove(4)

# Check if an element is in the set
if 5 in my_set:
    print("5 is in the set")

# Iterate over the elements of the set
for element in my_set:
    print(element)
```

# Listas

Uma lista normal, sem segredo.

```python
# Create a list
my_list = [1, 2, 3, 4, 5]

# Add an element to the list
my_list.append(6)

# Remove an element from the list
my_list.remove(4)

# Check if an element is in the list
if 5 in my_list:
    print("5 is in the list")

# Iterate over the elements of the list
for element in my_list:
    print(element)
```

# Dicionário/HashMap

Is an unordered collection of key-value pairs

```python
# Create a dictionary
my_dict = {"name": "Alice", "age": 30, "city": "New York"}

# Add a key-value pair to the dictionary
my_dict["country"] = "USA"

# Remove a key-value pair from the dictionary
del my_dict["age"]

# Check if a key is in the dictionary
if "name" in my_dict:
    print("name is in the dictionary")

# Iterate over the key-value pairs of the dictionary
for key, value in my_dict.items():
    print(key, value)

```
