# Data-structure-practical-program-17
class Stack:
    def __init__(self):
        self.stack = []

    def push(self, book_id):
        self.stack.append(book_id)
        print("Book ID", book_id, "added")

    def pop(self):
        if len(self.stack) == 0:
            print("Stack is empty")
        else:
            print("Removed Book ID:", self.stack.pop())

    def display(self):
        if len(self.stack) == 0:
            print("Stack is empty")
        else:
            print("Book IDs in Stack:", self.stack)

s = Stack()

s.push(101)
s.push(102)
s.push(103)

s.display()

s.pop()
s.display()
Book ID 101 added
Book ID 102 added
Book ID 103 added
Book IDs in Stack: [101, 102, 103]
Removed Book ID: 103
Book IDs in Stack: [101, 102]
