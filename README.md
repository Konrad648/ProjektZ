# Example program in Python: Simple calculator
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b != 0:
        return a / b
    else:
        return "Błąd: Dzielenie przez zero"

def main():
    print("Prosty kalkulator")
    print("Wybierz operację:")
    print("1. Dodawanie")
    print("2. Odejmowanie")
    print("3. Mnożenie")
    print("4. Dzielenie")

    choice = input("Wprowadź wybór (1/2/3/4): ")

    if choice in ['1', '2', '3', '4']:
        num1 = float(input("Podaj pierwszą liczbę: "))
        num2 = float(input("Podaj drugą liczbę: "))

        if choice == '1':
            print(f"Wynik: {add(num1, num2)}")
        elif choice == '2':
            print(f"Wynik: {subtract(num1, num2)}")
        elif choice == '3':
            print(f"Wynik: {multiply(num1, num2)}")
        elif choice == '4':
            print(f"Wynik: {divide(num1, num2)}")
    else:
        print("Nieprawidłowy wybór")

if __name__ == "__main__":
    main()
