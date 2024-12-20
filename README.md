Pizza Ordering System

Overview
This is a simple Java project designed to manage pizza orders with customizable options like adding extra cheese, extra toppings, and takeaway. It simplifies the process of calculating bills and ensures accurate pricing for every order.

Features
1.Customize Your Pizza
  *Choose between vegetarian or non-vegetarian pizza.
  *Add extra cheese and toppings to enhance your pizza.
  *Opt for takeaway with an additional backpack charge.
2.Automatic Pricing
  *Base prices for vegetarian and non-vegetarian pizzas are pre-defined.
  *Additional costs for cheese, toppings, and takeaway are automatically added to the total.
3.Generate Detailed Bills
  *Displays a breakdown of all charges, including base price, added items, and final bill amount.
4.DeluxPizza Option
  *A special pizza that comes with extra cheese and toppings pre-included for convenience.
5.File Handling (Planned for Extension)
  *Input: Ability to read orders from a file (future feature).
  *Output: Generate bills and save to a file (future feature).


Requirements
1.Java JDK
  *Ensure Java is installed (at least Java 8 or newer). Download it from Oracle's official website or use OpenJDK.
2.Code Editor
  *Use any code editor like Visual Studio Code, IntelliJ IDEA, or Eclipse.
  *Recommended extensions for VS Code: 
    ->Java Extension Pack
    ->Maven for Java
3.Git (Optional)
  *Use Git for version control and tracking changes.
4.GitHub (Optional)
  *Upload the project to GitHub to share it or keep it safe.


Project Structure
1. Main Class
  *Purpose: Orchestrates the program.
  *Functionality: 
    ->Creates pizza objects (Pizza or DeluxPizza).
    ->Demonstrates customization options (cheese, toppings, takeaway).
    ->Generates and displays the bill.
2. Pizza Class
  *Represents a customizable pizza order.
  *Attributes: 
    ->price (current total price of the pizza).
    ->veg (indicates if the pizza is vegetarian).
    ->extraCheesePrice, extraToppingsPrice, backPackPrice (constants for additional costs).
    ->basePizzaPrice (base price for the pizza).
    ->Flags for added cheese, toppings, or takeaway.
*Methods: 
    ->addExtraCheese(): Adds extra cheese to the pizza.
    ->addExtraToppings(): Adds extra toppings to the pizza.
    ->takeAway(): Adds a backpack for takeaway.
    ->getBill(): Displays a detailed breakdown of the charges.
3. DeluxPizza Class
  *Extends Pizza with pre-included extra cheese and toppings.
  *Methods: 
    ->Constructor: Automatically adds cheese and toppings to the pizza.
    ->Overrides customization methods (addExtraCheese, addExtraToppings) to disable further modifications.


Input and Output Structure (Planned for Extension)
Input File (input1.txt)
  *Contains pizza orders in the following format: 
  *Type, ExtraCheese, ExtraToppings, TakeAway
  *Veg,true,true,true
  *NonVeg,false,true,false
Output File (output.txt)
  *The program generates a detailed breakdown of bills for all orders.
  *Example Output: 
  *Pizza: 300
  *Extra cheese added: 100
  *Extra toppings added: 150
  *Take away: 20
  *Bill: 570

  *Pizza: 400
  *Extra toppings added: 150
  *Bill: 550


How to Run the Project
  1.Clone the repository: 
  2.git clone <repository-url>
  3.Compile and run the program: 
  4.javac Main.java
  5.java Main
  6.View the generated bills on the console. (File handling features will save outputs to output.txt in future updates.)

Why Use This Project?
This project is an easy-to-use system for managing pizza orders with detailed billing. It’s ideal for learning object-oriented programming concepts like inheritance, method overriding, and class design in Java while building a practical application.
