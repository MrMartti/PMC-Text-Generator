# PMC-Text-Generator
Training from Python Mega Course

import random, string
vowels='aieouy'
consonants='qwrtpsdfghjklzxcvbnm'
letters=string.ascii_lowercase
letter_input1=input("Choose some letters! 'v' for vowel, 'c' for consonts and 'a' for anything: ")
letter_input2=input("Choose some letters! 'v' for vowel, 'c' for consonts and 'a' for anything: ")
letter_input3=input("Choose some letters! 'v' for vowel, 'c' for consonts and 'a' for anything: ")

def generator():
    if letter_input1=='v':
        letter1=random.choice(vowels)
    elif letter_input1=='c':
        letter1=random.choice(consonants)
    elif letter_input1=='a':
        letter1=random.choice(letters)
    else:
        letter1=letter_input1
    if letter_input2=='v':
        letter2=random.choice(vowels)
    elif letter_input2=='c':
        letter2=random.choice(consonants)
    elif letter_input2=='a':
        letter2=random.choice(letters)
    else:
        letter2=letter_input2
    if letter_input3=='v':
        letter3=random.choice(vowels)
    elif letter_input3=='c':
        letter3=random.choice(consonants)
    elif letter_input3=='a':
        letter3=random.choice(letters)
    else:
        letter3=letter_input3
    name=letter1+letter2+letter3
    return(name)

for i in range(20):
    print (generator())
