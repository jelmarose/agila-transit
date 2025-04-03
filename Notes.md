# Notes

## Backend/Nest JS

### Terms to define:
- Module
- Controller - handles the HTTP requests
- Provider - handles the backend logic?
- Decorator
- Data Transfer Object (DTO) schema vs interface - DTO is for controllers while interface is for services i guess. every controller http request that handles an object needs it own dto file, like createTicketDto, updateTicketDto, compared to interface that just needs to define the Ticket object itself
- Dependency Injection - e.g services declared in the constructor of the controller

### Commands
- `npm run start:dev` - run nestjs localhost 
- `nest g module [name]` - creates new module inside [name] folder
- `nest g controller [name]` - creates new controller inside [name] folder
- `nest g service [name]` - creates new service inside [name] folder