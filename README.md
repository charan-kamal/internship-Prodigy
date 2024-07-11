#TASK1
def convert_temperature():
    temperature = float(input("Enter a temperature: "))
    unit = input("Enter the unit (C for Celsius, F for Fahrenheit, K for Kelvin): ")

    if unit.upper() == 'C':
        fahrenheit = (temperature * 9/5) + 32
        kelvin = temperature + 273.15
        print(f"{temperature} degrees Celsius is equal to {fahrenheit} degrees Fahrenheit and {kelvin} Kelvin.")

    elif unit.upper() == 'F':
        celsius = (temperature - 32) * 5/9
        kelvin = (temperature - 32) * 5/9 + 273.15
        print(f"{temperature} degrees Fahrenheit is equal to {celsius} degrees Celsius and {kelvin} Kelvin.")

    elif unit.upper() == 'K':
        celsius = temperature - 273.15
        fahrenheit = (temperature - 273.15) * 9/5 + 32
        print(f"{temperature} Kelvin is equal to {celsius} degrees Celsius and {fahrenheit} degrees Fahrenheit.")

    else:
        print("Invalid unit. Please enter C for Celsius, F for Fahrenheit, or K for Kelvin.")


convert_temperature()
