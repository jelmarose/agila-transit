### Trip Booking Flow
1. Select origin and destination terminal, departure date & number of guests
2. Generate a list of available trips based on a fixed timetable, displaying cabin selection
3. Ask for principal guest's details (full name, email, contact no)
4. Review order for confirmation
5. Ask for payment details (full name, country, postal code, address line 1 & 2, town/city)
6. Display pop up with fake credit card payment form (card number, month and year of expiration, CVV?)
7. Display success page.

### List of terminals

Luzon
- Laoag City
- Tuguegarao
- Santiago
- Baguio
- Dagupan
- Manila
- Batangas
- Lucena
- Naga 
- Legazpi City

Visayas
- Kalibo
- Roxas City
- Iloilo City
- Bacolod City 
- Sipalay City
- Dumaguete City
- Cebu City
- Bohol City
- Tacloban City
- Calbayog City

Mindanao
- Zamboanga
- Pagadian City
- Dipolog City
- Iligan City
- Cagayan de Oro
- Cotabato City
- Valencia City
- General Santos
- Davao City
- Butuan City

### Timetables

Fixed departure times:
- 06:00
- 09:00
- 12:00
- 15:00
- 18:00
- 21:00

Arrival times computation:
```typescript
    let distance = 0;
    let travelTimeInHrs = 0; 
    // Example: Baguio to Legazpi
    // Legazpi.id = 10, Baguio.id = 4
    distance = destinationTerminal.id - originTerminal.id;
    // distance is 6
    // get absolute value just in case the distance is negative
    distance = Math.abs(distance);

    if(distance < 3){
        travelTimeInHrs = 1 // default to 1 hr for simplicity
    }
    else if(distance < 6){
        travelTimeInHrs = 2
    }
    else{
        travelTimeInHrs = 3
    }
```