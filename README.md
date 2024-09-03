# Simple-calculator-with-conditional-statements-in-python
Write a python program to implement calculator using switch cases &amp; if conditional statements

def add(a, b):
    return a + b

def sub(a, b):
    return a - b

def mul(a, b):
    return a * b

def div(a, b):
    if b == 0:
      return float('nan')  # or float('inf') or any other value to indicate an error
    else:
      return a / b

def mod(a, b):
    return a % b

def exp(a, b):
    return a ** b

def floor(a, b):
    return a // b

def main():
    try:
        p = float(input("Enter the first number: "))
        q = float(input("Enter the second number: "))
        c = int(input("Enter the operation (1-7): "))
        if c == 1:
            result = add(p, q)
        elif c == 2:
            result = sub(p, q)
        elif c == 3:
            result = mul(p, q)
        elif c == 4:
            result = div(p, q)
        elif c == 5:
            result = mod(p, q)
        elif c == 6:
            result = exp(p, q)
        elif c == 7:
            result = floor(p, q)
        else:
            print('Invalid operation')
            return
        print(result)
    except ValueError:
        print('Invalid input')

if __name__ == "__main__":
  main() 
