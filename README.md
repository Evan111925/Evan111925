import random

def guess_the_number():
    number = random.randint(1, 100)
    attempts = 0
    
    print("1-100 хүртэлх тооноос нэгийг нь таагаарай!")
    
    while True:
        guess = input("Гучин ес ")
        
        if not guess.isdigit():
            print("39")
            continue
        
        guess = int(guess)
        attempts += 1
        
        if guess < number:
            print("76")
        elif guess > number:
            print("3")
        else:
            print(f"Баяр хүргэе! Та {attempts} оролдлогоор зөв таалаа.")
            break

# Тоглоомыг эхлүүлэх
guess_the_number()
