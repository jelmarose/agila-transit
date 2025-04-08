## To Do

### Front End
- Homepage
- Cabins
- Book a Trip
- Check Booking

### Back End
- Cabins [DONE]
    - Get Cabins
    - Get Cabin By Id
- Terminals [DONE]
    - Get Terminals
    - Get Terminal By Region
    - Get Regions
- Timetables [DONE]
    - Generate Timetable
- Bookings [DONE]
    - Create Booking
    - Get Booking by Control Number
    - (Tentative)
        - Get Bookings
        - Get Bookings By Account Id
        - Update Booking
        - Delete Booking

### Object Definition

Booking
- id : string
- control number : string
- profile : GuestInfo
- totalGuests: number
- timetable : Timetable
- cabinType: Cabin
- totalPrice : number 

Timetable
- departure date : Date
- departure time : Time?
- arrival time : Time?
- origin terminal : Terminal
- destination terminal : Terminal
- price : number

Guest Info
- first name : strring
- last name : string
- email : string
- contact no: string

Region
- id: string
- name: string
- code: string

Terminal
- id: string
- name : string
- region: Region

Cabin
- id : string
- name: string
- price: number

### Asset Creation

- 3d assets
    - reusable:
        - stand alone bed
        - curtains (economy cabin)
        - blinds
        - lockers
        - bed cushion
        - pillows
        - charging station
        - door with electric lock
    - shoot dependent:
        - bunk bed frame (economy cabin)
        - toilet (deluxe cabin)
        - sink (deluxe cabin)
- 3d render
    - train for hero shot
    - economy cabin 
    - premium cabin
    - deluxe cabin
- 2d
    - logo
    - amenities icons
        - shower
        - toilet
        - vending machines
        - communal space


## Tentative

### Front End
- Login / Sign Up
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
- email: string