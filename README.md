# avg-rainfall-calculator
limit = 12
month = 1
Q1, Q2, Q3, Q4 = 0,0,0,0
Max, Min = 0, 0
rain = 0
while(month <= limit):
    print("Enter RainFall for Month-",month,":", end='')
    rain = int(input())
    if(month <= 3):
        Q1 += rain
    elif(month <= 6):
        Q2 += rain
    elif(month <= 9):
        Q3 += rain
    else:
        Q4 += rain
    if(month == 1):
        Max = rain
        Min = rain
    
    if(rain > Max):
        Max = rain
    if(rain < Min):
        Min = rain
    month += 1

print("Average of Q1 : ",(Q1/3))
print("Average of Q1 : ",(Q2/3))
print("Average of Q1 : ",(Q3/3))
print("Average of Q1 : ",(Q4/3))

print("\nMaximum Rain Fall in a Month : ", Max)
print("\nMinimum Rain Fall in a Month : ", Min)
    
