# Stack Data Structure:
- Stack is a linear data structure which follows a particular order in which the operations are performed. 
- The order may be LIFO(Last In First Out) or FILO(First In Last Out).
Ex: Stack of Books
A
B
C
D
## Let's Code a Stack
- Python’s buil-in data structure list can be used as a stack

```python

class Stack():
    def __init__(self):
        self.items =[]
    def push(self,item):
        self.items.append(item)
    def pop(self):
        return self.items.pop()
    def get_stack(self):
        return self.items
    def isEmpty(self):
        return self.items ==[]

s = Stack()
# pushing A and B
s.push("A")
s.push("B")
print(s.get_stack())
# pushing C
s.push("C")
print(s.get_stack())
# popping,removing 
s.pop()
print(s.get_stack())

```