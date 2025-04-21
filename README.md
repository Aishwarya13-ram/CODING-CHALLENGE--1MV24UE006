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