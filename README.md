# restful-booker-postman-api-tests
Postman API test collection for Restful Booker including CRUD, authentication, and response validations.

# Restful Booker API Testing with Postman

This project contains API test scenarios for the Restful Booker API using Postman.

## Project Scope

The collection includes end-to-end API testing scenarios such as:

- Health check validation
- Authentication token creation
- Create booking
- Get created booking
- Full update booking with PUT
- Partial update booking with PATCH
- Delete booking
- Verify deleted booking with 404 response
- Status code validations
- Response body validations
- Environment variable usage
- API chaining with token and bookingId

## Tools Used

- Postman
- Restful Booker API
- JavaScript test scripts inside Postman

## Folder Structure

```text
collections/
  RestfulBooker.postman_collection.json

environments/
  RestfulBooker.postman_environment.json


How to Use
Import the collection file into Postman.
Import the environment file into Postman.
Select Restful Booker Env as the active environment.
Run the requests in the following order:
Health Check - Ping
Create Token
Create Booking
Get Created Booking
Update Booking
Partial Update Booking
Delete Booking
Get Deleted Booking - Verify Not Found

## Test Coverage

| Scenario               | Method | Expected Result |
| ---------------------- | ------ | --------------- |
| Health Check           | GET    | 201 Created     |
| Create Token           | POST   | 200 OK          |
| Create Booking         | POST   | 200 OK          |
| Get Booking            | GET    | 200 OK          |
| Update Booking         | PUT    | 200 OK          |
| Partial Update Booking | PATCH  | 200 OK          |
| Delete Booking         | DELETE | 201 Created     |
| Verify Deleted Booking | GET    | 404 Not Found   |

