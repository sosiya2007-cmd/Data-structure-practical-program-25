# Data-structure-practical-progr# Check balanced parentheses using stack

stack = []

expression = input("Enter expression: ")

balanced = True

for ch in expression:
    if ch == '(':
        stack.append(ch)
    elif ch == ')':
        if len(stack) == 0:
            balanced = False
            break
        stack.pop()

if balanced and len(stack) == 0:
    print("Balanced Parentheses")
else:
    print("Not Balanced")am-25
