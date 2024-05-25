import re

sum = 0
question = input("List or Individually? ")
if question.upper() == "INDIVIDUALLY":
    numCount = int(input("How many numbers did you want to average? "))
    for i in range(1, numCount+1):
        if i == 1:
            nextNumber = float(input("Enter the first number (number "+ str(i)+"): "))
            sum += nextNumber
        elif (1 < i < numCount):
            nextNumber = float(input("Enter the next number (number "+ str(i)+"): "))
            sum += nextNumber
        elif i == numCount:
            nextNumber = float(input("Enter the final number (number "+ str(i)+"): "))
            sum += nextNumber
    print("The average is ", sum/numCount)

elif question.upper() == "LIST":
    
    #Two options for the list input. This first one is worse, as once you commit to separating with a space or comma, you have stick with that choice
    #inList = (input("Enter your numbers ").replace(' ' , ',').split (','))

    #This one lets you mix and match, including putting as many commas or spaces as you want, but you have to import re
    inList = re.split(r'[,\s]+', input("Enter your numbers separated by commas or spaces: ").strip())
    
    for currentNumber in inList:
         sum += float(currentNumber)
    print("The average is " , sum/len(inList))
else: #error handling
    print("Invalid option selected")
