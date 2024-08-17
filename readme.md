Entities and Attributes
User

user_id (Primary Key)
name
email
address
phone_number
points
Bread

bread_id (Primary Key)
name
price
description
PaymentMethod

payment_method_id (Primary Key)
method_name
Transaction

transaction_id (Primary Key)
user_id (Foreign Key)
payment_method_id (Foreign Key)
total_price
transaction_date
TransactionItem

transaction_item_id (Primary Key)
transaction_id (Foreign Key)
bread_id (Foreign Key)
quantity
price
Ingredient

ingredient_id (Primary Key)
name
quantity_in_stock
unit
BreadIngredient

bread_ingredient_id (Primary Key)
bread_id (Foreign Key)
ingredient_id (Foreign Key)
quantity_used

