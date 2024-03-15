# CIS129_YourName_Lab5.py
    # CIS129 3/09/24
    # Robert Sickler
    # Bottle Return Program

    # Variables Declaration
    total_bottles = 0
    counter = 1
    today_bottles = 0
    total_payout = 0
    keep_going = "y"

    # Main Loop
    while keep_going.lower() == "y":
    # Setting Variable Values
    total_bottles = 0
    total_payout = 0

    # Input Loop
    for _ in range(7):
        print(f"Enter bottles for day #{counter}: ", end="")
        today_bottles = int(input())
        total_bottles += today_bottles
        counter += 1

    # Output
    total_payout = total_bottles * 0.10
    print("\nTotal bottles collected:", total_bottles)
    print("Total paid out: $", total_payout)

    # Continue or Exit Prompt
    print("\nDo you want to enter more data?")
    keep_going = input("(Enter y or n): ")
    
