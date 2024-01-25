import random
import string

def generate_password(length):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for i in range(length))
    return password

# Prompt the user for input
password_length = int(input("Enter the desired length of the password: "))

# Generate the password
generated_password = generate_password(password_length)

# Display the generated password
print("Generated Password:", generated_password)


print("Generated Password:", generated_password)
