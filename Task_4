import random

def determine_winner(user_choice, computer_choice):
    if user_choice == computer_choice:
        return "It's a tie!"
    elif (
        (user_choice == "rock" and computer_choice == "scissors") or
        (user_choice == "scissors" and computer_choice == "paper") or
        (user_choice == "paper" and computer_choice == "rock")
    ):
        return "You win!"
    else:
        return "You lose!"

def play_game():
    user_score = 0
    computer_score = 0

    while True:
        # Prompt the user for input
        user_choice = input("Enter your choice (rock, paper, scissors): ").lower()

        # Validate user input
        if user_choice not in ['rock', 'paper', 'scissors']:
            print("Invalid choice. Please enter rock, paper, or scissors.")
            continue

        # Generate computer's choice
        computer_choice = random.choice(['rock', 'paper', 'scissors'])

        # Determine the winner
        result = determine_winner(user_choice, computer_choice)

        # Display user's and computer's choices and the result
        print(f"\nYour choice: {user_choice}")
        print(f"Computer's choice: {computer_choice}")
        print(result)

        # Update scores
        if result == "You win!":
            user_score += 1
        elif result == "You lose!":
            computer_score += 1

        # Display current scores
        print(f"\nCurrent Scores:")
        print(f"You: {user_score}  Computer: {computer_score}")

        # Ask if the user wants to play again
        play_again = input("\nDo you want to play again? (yes/no): ").lower()
        if play_again != 'yes':
            break

# Start the game
play_game()

