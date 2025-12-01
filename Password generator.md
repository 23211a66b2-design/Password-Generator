```python
import random
import string

def generate_password(length):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = "".join(random.choice(characters) for _ in range(length))
    return password

def main():
    print(" PASSWORD GENERATOR (CODSOFT TASK 3)\n")
    
    try:
        length = int(input("Enter desired password length: "))
        
        if length <= 0:
            print("❌ Length must be greater than zero!")
            return
    except:
        print("❌ Invalid input! Enter a number.")
        return

    password = generate_password(length)
    print("\n✅ Your Generated Password:")
    print("👉", password)

main()

```

     PASSWORD GENERATOR (CODSOFT TASK 3)
    
    

    Enter desired password length:  8
    

    
    ✅ Your Generated Password:
    👉 vG)@VEmF
    


```python

```
