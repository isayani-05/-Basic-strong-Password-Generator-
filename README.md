# 🔐 Basic Strong Password Generator
"This is a simple Python-based strong password generator designed to create secure, random passwords for general use. It allows users to generate passwords of customizable length using a mix of ascii, uppercase and lowercase letters, numbers, and special characters. The generator helps promote good password hygiene by ensuring high entropy and resistance to brute-force attacks."

from random import  *
import string

n=int(input("Enter password length: "))

a=string.ascii_uppercase
b=string.ascii_lowercase
c=string.punctuation
d=string.digits

chrs=a+b+c+d

pwd="".join(sample(chrs, n))

print(f"Random password of {n} characters: {pwd}")
    
