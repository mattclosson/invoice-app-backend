# Invoice App 

## User Stories
User will be able to login/signup and connect their account to Stripe Connect
Users will be able to create an invoice and send to their customer
Customer can pay for the invoice via Stripe
Users will be able to manage their invoices

## Stack
- MongoDB
- Express.JS
- Svelte
- Stripe.JS
- Email.JS

## Models
User: 
  - username: String,
  - password: String,
  - stripeAccountId: String


Invoice:
  - userId: String,
  - paymentDue: Date,
  - total: Number,
  - paid: Boolean,
  - description: String
  
## Routes
|               |               |
| ------------- | ------------- |
| /user | Create         |
| /user | Get All Users  |
| /user/id | Get User    |
| /user/id | Update User |
| /user/id | Delete User |
| /invoice | Create        |
| /invoice | Get All Invoices |
| /invoice/id | Get Invoice      |
| /invoice/id | Update Invoice   |
| /invoice/id | Delete Invoice   |
| /user/invoice/ | Get All User Invoices |
| /user/invoice/id | Get User Invoice    |
