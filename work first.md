```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[6], line 5
          3         self.data = data
          4         self.next = None
    ----> 5 print(traverse_all(Node))
    

    NameError: name 'traverse_all' is not defined



```python
class LinkedList:
    def __init__(self):
        dummy = Node("dummy")
        self.head = dummy
        self.tail = dummy

        self.current = None
        self.before = None

        self.num_of_data = 0
    def append(self, data):
        new_node = Node(data)
        self.tail.next = new_node
        self.tail = new_node
        self.num_of_data += 1
```


```python
    def delete(self):
        pop_data = self.current.data

        if self.current is self.tail:
            self.tail = self.before
            self.before.next = self.current.next
            self.current = self.before 
            self.num_of_data -= 1
            return pop_data
```


```python
     def first(self):
        if self.num_of_data == 0: 
            return None

        self.before = self.head
        self.current = self.head.next

        return self.current.data

```


```python
       if data:
        print(data, end=' ')
        while True:
            data = l_list.next()
        else:
            print(data, end= ' ')
        
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[18], line 1
    ----> 1 if data:
          2  print(data, end=' ')
          3  while True:
    

    NameError: name 'data' is not defined



```python
      
```


      Cell In[15], line 1
        def data = l_list.first():
                 ^
    SyntaxError: invalid syntax
    



```python
       if data:
        print(data, end=' ')
        while True:
            data = l_list.next()
        if data:
            print(data, end= ' ')
        else:
            break
```


      Cell In[16], line 8
        break
        ^
    SyntaxError: 'break' outside loop
    



```python

```
