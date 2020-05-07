
# [A Database Design for Book Store](https://github.com/oloolaa/Database-Design "A Database Design for Book Store")

## Introduction
The design of this database for a bookstore is based on examples like Barnes & Noble and Amazon Kindle Store, and thus we are going to include the features not only from a traditional book store but also from an online book store. Besides the basic features, there are some important features such as:
1. Book genres: Fiction, Literature, Mystery & Crime, Romance, Poetry, Art, Architecture & Photography, Business Books, etc.
2. Book department: Newspaper, Magazine, Kids & Teens, etc.
3. Book reviews.
4. Online shopping cart.
5. User's online information. The "user" category includes normal users and administrators.
6. Customer's discounts
7. Book discounts.
8. Payment method.
9. Shipping records.
10. Payment records.
11. etc.


## Assumptions
1. An account can only be a customer or an administrator. A customer can place an order, put items into his/her shopping cart, use the discounts he/she owns to make an order, and make reviews of the books. Administrators are not allowed to make orders but can only audit the existing orders and add PL/SQL operations.
2. A discount can be eligible for a group of users or books, and thus for entity "Book" and entity "Account", there should be an attribute indicating which discount it has. When an order is placed, only one discount will be effective, which is up to the customer's choice. A customer will be able to choose whether to use his/her own discount to apply to all books in the shopping cart, otherwise only the discounts for books will be effective.
3. A book can belong to several genres, while it can only belong to one department.
4. For the payment methods of every order, there are three available methods for our database, which are "BankAccount", "GiftCard", and "EPay". Besides the basic attributes for the payment, each of these methods has its own attributes.
5. A book has reviews made by different customers. And one customer can make reviews for different books.
6. The shipment information for every order is also tracked by ShipmentID, ShipmentDate and ShipmentFee and the address to deliver.


## EER Diagram
Enough of the words, one picture is good enough to show it all.
[![EER Diagram](https://raw.githubusercontent.com/oloolaa/Database-Design/master/EER%20Diagram.png "EER Diagram")](https://raw.githubusercontent.com/oloolaa/Database-Design/master/EER%20Diagram.png "EER Diagram")
