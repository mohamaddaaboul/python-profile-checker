# python-profile-checkerdef main():
    # Collect user input
    name = input("Enter your name: ")
    age = int(input("Enter your age: "))
    gpa = float(input("Enter your GPA (0.0 - 5.0): "))
    field = input("Enter your field of interest: ")
    graduated = input("Have you graduated? (yes or no): ").strip().lower()

    # Print nicely formatted info
    print("\n=== User Profile ===")
    print(f"Name            : {name}")
    print(f"Age             : {age}")
    print(f"GPA             : {gpa}")
    print(f"Field of Interest: {field}")
    print(f"Graduated       : {graduated.capitalize()}")
    print("====================")

    # Decision logic
    if age < 25 and gpa >= 3.5 and graduated == "yes":
        print("\n✅ You are eligible for a *scholarship*.")
    elif age < 30 and gpa >= 2.5:
        print("\n✅ You are eligible for an *internship*.")
    else:
        print("\n❌ You are not eligible currently. Please apply again later.")

if _name_ == "_main_":
    main()
