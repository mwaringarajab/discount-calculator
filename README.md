# discount-calculator

A simple Python script that calculates the final price of an item after applying a discount. If the discount is 20% or more, it is applied to the original price; otherwise, the original price is returned unchanged.

## Features

- Calculates the final price based on user input.
- Applies discount only if it is **20% or more**.
- Handles invalid inputs with user-friendly message.

## Requirements

- Python 3.x

## How to Run

1. Clone or download this repository.
2. Open your terminal or command prompt.
3. Navigate to the folder where the script is saved.
4. Run the script using:

```bash
python discount_calculator.py

Example Usage
Enter the original price of the item: 1000
Enter the discount percentage: 25
Discount applied. Final price: 750.00

Enter the original price of the item: 500
Enter the discount percentage: 15
No discount applied. Final price: 500.00
Function Used
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        return price - discount_amount
    else:
        return price