# BULK PURCHASE APP

Web application based on MERN stack - MongoDB, Express.js, React.js, and Node.js.

## HOW TO RUN

In another terminal, run the backend
```
cd backend
npm install
npm start
```

In another terminal, run the frontend
```
cd frontend
npm install
npm start
```

For this assignment, you are required to make a web app with:

- Frontend in ​React.js
- Backend using ​Express.js​ which implements a ​REST​ API
- Database in ​MongoDB

## USE CASES

### 1. USER MANAGEMENT

There are two types of users - Vendors and Customers. Each of them have their own use-cases

### 1.1. LOGIN PAGE

It has an option to enter the username and password, and then login. There is also an option to register in case the user does not have an existing account.

#### 1.2. REGISTRATION PAGE

During registration, there would be the option to select between customer and vendor type. Here the user enters his full name, email address, phone number, address etc etc.

### 2. VENDOR USE CASES

#### 2.1. CREATE NEW PRODUCT

Create a new product specifying its Name, Price, and Quantity in the Bundle

#### 2.2. VIEW ALL PRODUCTS ISSUED BY HIM/HER

Should be able to view all the current product listing done by him/her

- There should be an option to take down a listing making sure that customers get their product status as canceled.
- Once the product is ready to dispatch (i.e. when it has been ordered bysufficient people), it is removed from this view and becomes ready todispatch

#### 2.4. VIEW ALL ORDERS READY TO DISPATCH

Should have a button to dispatch the product which removes it from this view.

#### 2.5. VIEW ALL DISPATCHED ORDERS WITH REVIEWS AND RATINGS PER ORDER

All dispatched orders should be displayed in another view with the reviews and ratings of each order.

### 3. CUSTOMER USE CASES

#### 3.1. SEARCH FOR PRODUCT

- Exact string matching would do
- All the vendors selling that product should be displayed along with their price and quantity remaining
- sort by price or quantity of items remaining or rating of the seller (<https://www.c-sharpcorner.com/UploadFile/fc34aa/sort-json-object-array-based-on-a-key-attribute-in-javascrip/> done on front end)

#### 3.2. ORDER PRODUCT

- select product
- specify quantity desired
- place order

#### 3.3. VIEW ORDER STATUS

- dispatch status {Waiting,Placed,Dispatched,Canceled}
  - Waiting (If not enough orders have been placed meeting the minimum bulk quantity requirement by the seller)
    - Quantity left for the order to get placed
    - Option to edit the order if not in the dispatched state
  - Placed (If the quantity requirements are met but is yet to get dispatched by the seller in his/her portal)
    - Rate vendor
  - Dispatched (If the seller accepts the order in his/her portal)
    - give a product review along with a rating once theproduct has been dispatched.
  - Canceled (If the seller cancels the order in his/her portal)



Navigate to localhost:3000/ in your browser.
