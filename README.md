import random

secret = random.randint(1, 10)
attempts = 0

print("გამოიცანი რიცხვი 1-დან 10-მდე")

while True:
    guess = int(input("შეიყვანე რიცხვი: "))
    attempts += 1

    if guess == secret:
        print(f"გილოცავ! გამოიცანი {attempts} ცდაში 🎉")
        break
    elif guess < secret:
        print("უფრო დიდი რიცხვია ⬆️")
    else:
        print("უფრო პატარა რიცხვია ⬇️")
