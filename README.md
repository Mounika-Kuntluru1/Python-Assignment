# Python-Assignment
Task 1- Calculate Area with Conditions
Write a Python function calculate_area that takes two parameters: length and width. It
should calculate and return the area of a rectangle. However, add a condition: if the length
is equal to the width, return "This is a square!" instead of the area. Then, write a program to input 
values for length and width from the user and call the calculate_area function to
display either the area or the message.
Code
def calculate_area(length, width):
 if length == width:
 return "This is a square!"
 else:
 return length * width
def main():
 try:
 length = float(input("Enter the length of the rectangle: "))
 width = float(input("Enter the width of the rectangle: "))
 result = calculate_area(length, width)
 if isinstance(result, str): 
 print(result)
 else:
 print(f"The area of the rectangle is: {result}")
 except ValueError:
 print("Invalid input. Please enter valid numerical values for length and width.")
if __name__ == "__main__":
 main()


 
