import random

def generate_question(table_number):
    multiplier = random.randint(1, 10)
    correct_answer = table_number * multiplier
    return multiplier, correct_answer

def multiplication_exam():
    print("Welcome to the Kids Multiplication Table Exam!\n")
    table_number = int(input("Enter the multiplication table you want to practice (e.g., 2, 3, 5): "))
    num_questions = int(input("How many questions do you want Dingu? "))

    score = 0

    for i in range(1, num_questions + 1):
        multiplier, correct_answer = generate_question(table_number)
        try:
            user_answer = int(input(f"Q{i}: What is {table_number} x {multiplier}? "))
            if user_answer == correct_answer:
                print("Correct Dingu!\n")
                score += 1
            else:
                print(f"Wrong Dingu. The correct answer is {correct_answer}.\n")
        except ValueError:
            print(f"Invalid input. The correct answer was {correct_answer}.\n")

    print(f"Exam finished! Your score: {score}/{num_questions}")

if __name__ == "__main__":
    multiplication_exam()
