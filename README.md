# Python-Code-Samples
#Giselle Rodriguez
#10.11.23

#Problem 1
#program that prints Hello World
print("Hello World")

#Problem 2
#program that asks user for their name and greets them
name = input("Hello what is your name?")
#print your name
print("Hello " + name + " it's nice to meet you"+ "!")

#Problem 3
#modified program that only greets user and instructor 
#list user and instructor names
greeting_names= ["giselle", "ms. likoudis"]
#ask the user for their name
name = input("What is your name? ")
#check if the greeting names are valid
if name.lower() in greeting_names:
    #greet the user by their name
    print(f"Hello, {greeting_names}!")
else:
    #do not greet user
    print("Sorry, only able to greet user and instructor")

#Problem 4
#program that computes the area of a circle
pi= 3.14159
#enter the radius
radius = float(input("Enter radius of circle"))
area = pi * (radius ** 2)
#print user a nice message with answer
print(f"The area of the cirle with radius {radius} is {area:.2f}.")

#Problem 5
#program that computes MPG for a car
#function
#enter the number of miles driven
Miles = float(input("Enter the number of miles driven"))
#enter the number of gallons used
Gallons = float(input("Enter the number of gallons used"))
#MPG calculation
MPG = Miles / Gallons
print(f"The car's MPG is {MPG:.2f}.")

#Problem 6
#program that convers Fahrenheit to Celsius degrees
#function
def fahrenheit_to_celsius(fahrenheit):
    celsius = (fahrenheit - 32) * 5 / 9
    return celsius
#enter the temperature in Fahrenheit
fahrenheit = float(input("Enter the temperature in Fahrenheit: "))
#convert to celsius
celsius = fahrenheit_to_celsius(fahrenheit)
#print message with answer
print(f"The temperature in Celsius is: {celsius}")

#Problem 7
#program that asks for the starting day number, the length of stay, and will tell you the number of day of the week you will return by
def day_name(x):
    days = { 
0: 'Sunday',
1: 'Monday', 
2: 'Tuesday',
3: 'Wednesday', 
4: 'Thursday',
5: 'Friday',
6: 'Saturday',
}
#enter the starting day
starting_day_str = input("What day are you starting on?")
#enter the length of stay
length_of_stay_str = input("How long are you staying?")
#variables
starting_day_int = int(starting_day_str)
length_of_stay_int = int(length_of_stay_str)
#function
computing_length = starting_day_int + length_of_stay_int
returning_on_day = computing_length - 7
#print message with day the user will be back
print(returning_on_day)
