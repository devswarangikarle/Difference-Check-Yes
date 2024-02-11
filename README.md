# Difference-Check-Yes
You're given three integers (num1, num2, num3), you need to determine whether one of the numbers is the difference between the other two numbers. If such a number exists, return "Yes". Otherwise, return "No".

def is_difference(num1, num2, num3):
    if num1 - num2 == num3 or num2 - num1 == num3:
        return "Yes"
    elif num2 - num3 == num1 or num3 - num2 == num1:
        return "Yes"
    elif num1 - num3 == num2 or num3 - num1 == num2:
        return "Yes"
    else:
        return "No"


num1, num2, num3 = map(int, input().split())


result = is_difference(num1, num2, num3)
print(result)
