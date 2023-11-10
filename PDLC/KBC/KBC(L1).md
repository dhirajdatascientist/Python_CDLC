### KBC(L1)

```
# KBC Program

def ask_question(question, correct_answer):
    """
    Function to ask a question and check the answer.
    """
    user_answer = input(question + " ")
    if user_answer.lower() == correct_answer.lower():
        print("Correct!")
    else:
        print("Incorrect. The correct answer is:", correct_answer)

def main():
    # Question 1
    question1 = "What is the capital of France?"
    answer1 = "Paris"
    ask_question(question1, answer1)

    # Question 2
    question2 = "What is the largest planet in our Solar System?"
    answer2 = "Jupiter"
    ask_question(question2, answer2)

if __name__ == "__main__":
    main()

```