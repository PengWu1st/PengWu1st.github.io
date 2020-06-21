---
layout: post
title: "data structure in python"
---
# 用python实现栈

```python
class Stack:
    def __init__(self):
        self.items = []
    
    def is_empty(self):
        return bool(self.items)
    
    def push(self, item):
        self.items.append(item)
        
    def peek(self):
        self.items[-1]
        
    def size(self):
        return len(self.items)
    
    def pop(self):
        return self.items.pop()
```

应用举例：浏览器回退

# 用python实现队列

```python
class Queue:
    def __init__(self):
        self.items = []
    
    def is_empty(self):
        return bool(self.items)
    
    def enqueue(self, item):
        self.items.insert(0, item)
        
    def dequeue(self):
        self.items.pop()
        
    def size(self):
        return len(self.items)
    
```

应用举例：任务队列

# 用python实现双端队列

```python
class Deque:
    def __init__(self):
        self.items = []
    
    def is_empty(self):
        return bool(self.items)
    
    def add_front(self, item):
        self.items.append(item)
        
    def add_rear(self, item):
        self.items.insert(0, item)

    def remove_front(self)
        return self.item.pop()

    def remove_rear(self)
        return self.item.pop(0)

    def size(self):
        return len(self.items)
    
```

应用举例：回文检测

# 用python链表实现无序列表
```python
class Node:
    def __init__(self, init_data):
        self.data = init_data
        self.next = None
    
    def get_data():
        return self.data

    def get_next():
        return self.next
    
    def set_data(new_data):
        self.data = new_data
    
    def set_next(new_next)：
        self.next = new_next

class UnorderedList：

    def __init__(self):
        self.head = None

    def is_empty(self):
        return self.head is None
    
    def add(self, data):
        temp = Node(data)
        temp.set_next(self.head)
        self.head = temp
    
    def length(self):
        count = 0
        current = self.head
        while current is not None:
            count += 1
            current = current.get_next()
        return count


```