# CODING-CHALLENGE-1MV24UE006
def count_vowels_and_consonants(input_string):
    vowels = set("aeiou")
    consonants = set("bcdfghjklmnpqrstvwxyz")
    vowel_count = 0
    consonant_count = 0
    input_string = input_string.lower()
    for char in input_string:
        if char in vowels:
            vowel_count += 1
        elif char in consonants:
            consonant_count += 1
    print(f"Number of vowels: {vowel_count}")
    print(f"Number of consonants: {consonant_count}")

# Input from the user
input_string = input("Enter a string: ")
count_vowels_and_consonants(input_string)

Output 
Enter the number of Fibonacci numbers to print: 7
First 7 Fibonacci numbers: [0, 1, 1, 2, 3, 5, 8]

def is_prime(num):
    # Function to check if a number is prime
    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

def print_primes_upto_n(n):
    # Check if the input is valid
    if n < 2:
        print("There are no prime numbers less than or equal to", n)
        return
    
    # Find and print all prime numbers less than or equal to n
    primes = [num for num in range(2, n + 1) if is_prime(num)]
    print(f"Prime numbers less than or equal to {n}: {primes}")

# Input from the user
try:
    n = int(input("Enter an integer n: "))
    print_primes_upto_n(n)
except ValueError:
    print("Please enter a valid integer.")

Enter an integer n: 10

Prime numbers less than or equal to 10: [2, 3, 5, 7]