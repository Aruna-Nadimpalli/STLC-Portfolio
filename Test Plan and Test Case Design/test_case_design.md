# Test Cases for GroceryMate
The following test cases are based on the new features that will be developed for the upcoming release of the grocery shop application.

**Software**: http://grocerymate.masterschool.com
 
## Feature:  Age Verification for Alcoholic Products
**Test case design techniques:**  Boundary value analysis, Equivalence partitioning, Error Guessing
### Test Cases
**Boundary value analysis**
- Test case: Verify account creation for a user exactly 18years old
	- Input: Date of birth (Today 18 years old)
	- Expected Outcome: Account creation Successful.

**Boundary value analysis**
 - Test case: Verify account creation for a user just below 18 years old
	- Input : Date of birth (Today - 18 years- 1 day)
	- Expected out come: Error message " You must be at least 18 years old to create an account.

**Equivalence partitioning**
- Test case : Verify account creation for user below the age of 18.
    - Input: Date of birth (Today -17 years)
    - Expected outcome: Error message displayed

**Equivalence partitioning**
- Test case: Verify the account creation for users above the age of 18
    -Input: Date of birth ( Today - 19 years old)
    -Expected out come: Account creation successful:

**Error guessing**
- Test case: verify system behaviour when date of birth is not entered.
    - Input: Date of birth field left empty.
    - Expected outcome: Error message "Date of birth required"

**Error guessing**
- Test case: Verify the system behaviour when an invalid date of birth format is entered
    - Input: Date of birth "07201983"
    - Expected outcome: Error message "Invalid date of birth format" please use MM/DD/YYYY.



## Feature: Shipping cost changes

**Test Design Techniques**
 Boundary Value Analysis,  Equivalence Partitioning,Error Guessing.

### Boundary Value Analysis
- Test Case Verify that free shipping is applied if the products price is more or equal to 20 euros
    - Input: Add items to the cart, so that total items cost exceed 20 euro
    - Expected outcome: Free shipping facility applied.

- Test case: Verify that whether free shipping is applied if the total items in shipping cart is less than 20 euro.
    -  Input: Add items to the shipping cart, so that the total price of the items is less than 20 euros.
    -  Expected out come: Shipping fee 5 euros is applied.

### Error Guessing:
- Test case: Verify that the shipping fee is applied when the items are removed from the cart, and the total cost becomes less than 20 euros.
    - Input: Add products then try to remove the items from the shipping cart, so that the total cost of the items is less than 20 euros.
    - Expected outcome: shipping fee is applied correctly based on new total cost.

- Test case: Verify that the shipping cost is free when the quantity of items is increased from the cart and the total cost is more than 20 euros,
    - Input: Add items, then try increasing the quantity of the items from cart, so that the total cost becomes more than 20 euros.
    - Expected outcome: Free shipping is applicable.

## Feature: Product Rating System**
**Test design techniques:**
Boundary value analysis,Equivalence partitioning,Error guessing.

### Boundary value analysis
- Test case:verify that product rating is applied if the rating given as 5 star
    - Input: Give the product rating as 5 stars to the product
    - Expected out come: 5 star rating is visible beneath the product

- Test case: Verify that product rating is applied if the rating given as 3 stars.
    - Input: Give the product rating as 3 stars to the product.
    - Expected outcome:3 star rating is visible beneath the product.

- Test case:verify that product rating is applied if the rating given as none
    - Input: Never rate the product.
    - Expected outcome: Invalid rating is showing on the screen.
