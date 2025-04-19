# Restaurant-Menu
#define the menu of a hotel 
menu = {
    'pizza': 40,
    'pasta': 30,
    'burger':60,
    'cake': 15
}
#Greet
print("Welcome to the Python restaurant!")
print("We have the following items in our menu:")
print("pizza: Rs40\npasta: Rs30\nburger: Rs60\ncake: Rs15\n")

order_total= 0

item_1 = input("Enter your first item to order:")
if item_1 in menu:
    order_total+= menu[item_1]
    print(f"Your item {item_1} is added to your order")

else:
    print(f"Sorry, ordered item {item_1} is not in the menu yet!")
    

another_order = input("Do you want to order another item? (Yes/No): ")
if another_order.lower() == "yes":
    item_2 = input("Enter your second item to order:")
    if item_2 in menu:
        order_total += menu[item_2]
        print(f"Your item {item_2} is added to your order")
    else:
        print(f"Order item {item_2} is not in menu yet")

    print(f"Your total order is Rs{order_total}")
