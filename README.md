# discount_-python
def calculate_discount(price, discount_percent):
    # Check if the discount is 20% or higher
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        final_price = price - discount_amount
        return final_price
    else:
        return price

# Prompting user for input
original_price = float(input("Enter the original price of the item: "))
discount_percentage = float(input("Enter the discount percentage: "))

# Calculating final price
final_price = calculate_discount(original_price, discount_percentage)

# Printing the result
if final_price == original_price:
    print(f"No discount applied. Original price: ${original_price:.2f}")
else:
    print(f"Final price after applying the discount: ${final_price:.2f}")
