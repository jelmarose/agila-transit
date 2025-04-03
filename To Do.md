## To Do

### Front End
- Homepage
- Login / Sign Up
- Place Order 
- Check Order Status
- Profile

### Back End
- Tickets
    - Get Tickets
    - Get Ticket By Id
- Orders
    - Get Orders
    - Get Order By Id
    - Get Order By Control Number
    - Get Orders By Account Id
    - Create Order
    - Update Order
    - Delete Order
- Payment Type
    - Get Payment Types
- Accounts
    - Get Accounts
    - Get Account By Id
    - Update Account
    - Delete Account
- Profiles
    - Get Profile By Id
    - Create Profile
    - Update Profile
    - Delete Profile

### Object Definition

Account
- id : string
- email : string
- password : string
- profile id : string

Profile
- id : string
- account id : string
- first name : string
- last name : string
- contact number : string

Order
- id : string
- control number : string
- is guest : boolean
- profile : Profile (account id is just 00000 if guest)
- tickets (array)
    - ticket : Ticket
    - quantity : number
- payment type : Payment Type

Payment Type
- id: string
- name: string

Ticket
- id : string
- name: string
- price: number