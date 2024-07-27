# Pizza Bill Generator

This project is a simple Java application that simulates a pizza billing system. It includes classes to handle different types of pizzas, additional toppings, and extra services like takeaways. 
The application calculates the final bill based on the selected options and provides a detailed bill.

## Features

- Base pizza prices for vegetarian and non-vegetarian options.
- Options to add extra cheese and extra toppings.
- Option for takeaway.
- Deluxe pizza option which automatically includes extra cheese and extra toppings.

## Classes

### `pizza`

This class represents a basic pizza with options for extra cheese, extra toppings, and takeaway.

- **Attributes**:
  - `price`: The current price of the pizza.
  - `veg`: Boolean indicating if the pizza is vegetarian.
  - `extraCheesePrice`: Cost of adding extra cheese.
  - `extraToppingsPrice`: Cost of adding extra toppings.
  - `takeAwayPrice`: Cost of takeaway.
  - `basePizzaPrice`: The base price of the pizza.
  - `isExtraCheeseAdded`: Boolean indicating if extra cheese is added.
  - `isExtraToppingsAdded`: Boolean indicating if extra toppings are added.
  - `isOptedForTakeAway`: Boolean indicating if takeaway is opted.

- **Methods**:
  - `pizza(boolean veg)`: Constructor to initialize the pizza with base price.
  - `addExtraCheese()`: Adds extra cheese to the pizza.
  - `addExtraToppings()`: Adds extra toppings to the pizza.
  - `takeAway()`: Adds takeaway option to the pizza.
  - `getBill()`: Prints the detailed bill.

### `DeluxPizza`

This class extends the `pizza` class and represents a deluxe pizza which includes extra cheese and extra toppings by default.

- **Methods**:
  - `DeluxPizza(boolean veg)`: Constructor to initialize the deluxe pizza.
  - `addExtraCheese()`: Overridden method to prevent adding extra cheese.
  - `addExtraToppings()`: Overridden method to prevent adding extra toppings.

### `main`

This class contains the `main` method to run the application.

- **Methods**:
  - `main(String[] args)`: Main method to create and test the pizza objects.
