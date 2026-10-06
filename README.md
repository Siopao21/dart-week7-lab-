# dart-week7-lab-
# Week 7 Lab – Dart Fundamentals

Name: Bern Cortes
Section: BSIT 3.7

## Files

- campus_brew_receipt.dart – Campus Brew order receipt (Parts 2–8)
- print_shop.dart – Campus Print Shop bill (Part 10)

## How to run

Copy a file's code into https://dartpad.dev and click Run.

## Part 7 answers

1. Ana got the student voucher because she is a student and her subtotal is at least PHP 250.

2. Delivery was not free because after the voucher, the total was PHP 281.25, which is below the PHP 300 free delivery minimum, and she was not picking up the order.

3. We use ~/ instead of / for points because ~/ gives only the whole-number result.

## Part 8 results table

| Order | Student voucher | Delivery | TOTAL | Change | Points |
|---|---|---|---|---|---|
| A — Ana | -PHP 15.50 | PHP 29.50 | PHP 310.75 | PHP 89.25 | 6 |
| A with isStudent = false | Not eligible | FREE | PHP 326.25 | PHP 73.75 | 6 |
| B — Ben | Not eligible | FREE | PHP 295.75 | PHP 4.25 | 5 |
| C — Carla | -PHP 15.50 | FREE | PHP 321.00 | PHP 179.00 | 6 |

Carla got free delivery because after the student voucher, her total was PHP 321.00, which is above the PHP 300 free delivery minimum.

## Part 9 debugging table

| Bug | What was wrong | Your fixed line |
|---|---|---|
| 1 | Missing semicolon | `String drink = 'Iced Coffee';` |
| 2 | A decimal value was assigned to an int | `double price = 65.25;` |
| 3 | A final variable was reassigned | `String shop = 'Campus Brew';` |
| 4 | The multiplication was printed instead of calculated | `double total = price * qty;` |
| 5 | Division used `/` instead of whole-number division | `int boxes = cups ~/ 6;` |

## Part 10 test results

| Test | Student Name | blackPages | colorPages | isMember | wantsBinding | Member discount | TOTAL | Minutes |
|---|---|---:|---:|---|---|---|---:|---:|
| 1 | Ana Reyes | 24 | 6 | true | true | -PHP 5.25 | PHP 140.00 | 3 |
| 2 | Ben Cruz | 14 | 2 | false | false | Not eligible | PHP 51.50 | 2 |
| 3 | Carla Santos | 30 | 1 | true | false | Not eligible | PHP 83.25 | 3 |

Carla does not get the member discount because her subtotal is PHP 83.25, which is below the PHP 100 minimum.

## Reflection

1. The error message that confused me the most was the type error because I initially used the wrong data type. I fixed it by checking the value and changing the variable to the correct type.

2. `final` would be a better choice for values that should not change while the receipt is running, such as the customer name or fixed values that are only assigned once.

3. In a real Flutter app, the INPUT values would come from things like text fields, buttons, or other user interface controls.
