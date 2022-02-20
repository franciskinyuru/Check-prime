# Check-prime
# a number is considered prime if its divisible by one or itself.

#method 1.
# define a variable to keep status:
check = False

# input number to check if its prime.
num = input("Enter number to check if its prime: ")

# prime numbers are greater than 1

if (int(num) > 1):
# check for factors
    for i in range(2, int(num)):
# if factor is found, set check to True
        if (int(num) % i) == 0:
            check = True
# break out of loop
            break

# check if flag is True
if check:
    print("The number {}".format(num) + " is not prime")
else:
    print("The number {}".format(num) + " is prime")


# method 2

if int(num) > 1:
#  check for factors
    for i in range(2, int(num)):
# check for factors
        if (int(num) % i) == 0:
            print("The number {}".format(num) + " is not prime")
        else:
            print("The number {}".format(num) + " is prime")
else:
# if number is less than one or equal to one
    print("The number {}".format(num) + " is not prime")

