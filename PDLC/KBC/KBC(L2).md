### KBC(L2)
```
def login():
    """
    Function to handle user login.
    """
    username = input("Enter username: ")
    password = input("Enter password: ")
    if username == "admin" and password == "admin":
        return True
    else:
        print("Invalid credentials.")
        return False

def ask_question(question, correct_answer):
    """
    Function to ask a question and check the answer.
    Returns True if the answer is correct, else False.
    """
    user_answer = input(question + " ")
    if user_answer.lower() == correct_answer.lower():
        print("Correct!")
        return True
    else:
        print("Incorrect. The correct answer is:", correct_answer)
        return False

def main():
    # Login
    if not login():
        return

    score = 0

    # Question 1
    question1 = "What is the capital of France?"
    answer1 = "Paris"
    if ask_question(question1, answer1):
        score += 1000
    else:
        score -= 1000

    # Question 2
    question2 = "What is the largest planet in our Solar System?"
    answer2 = "Jupiter"
    if ask_question(question2, answer2):
        score += 1000
    else:
        score -= 1000

    print("Your final score is: ₹", score)

if __name__ == "__main__":
    main()
```