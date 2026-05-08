# Restful Booker — Hotel Booking API Test Suite

![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white)
![Assertions](https://img.shields.io/badge/Assertions-53%20Passed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

End-to-end API test collection for the Restful Booker Hotel Booking API built with Postman — covering 15 test cases and 53 assertions across authentication, CRUD operations and negative/security testing.

**Prepared by:** Abdul Hannan — SQA Engineer
**API Under Test:** https://restful-booker.herokuapp.com

---

## Test Results Summary

| Metric | Value |
|---|---|
| Total Requests | 15 |
| Total Assertions | 53 |
| Passed | 53 ✅ |
| Failed | 0 ✅ |
| Duration | ~7 seconds |

---

## Test Coverage

| Module | TCs | Assertions | Test Types |
|---|---|---|---|
| Health Check | 1 | 3 | Availability, response time |
| Authentication | 2 | 7 | Valid login, invalid credentials |
| Booking GET Operations | 4 | 18 | Get all, by ID, filters, negative |
| Booking POST/PUT/PATCH/DELETE | 7 | 25 | Create, update, delete, security |
| **Total** | **15** | **53** | All passed |

---

## Endpoints Covered

| Method | Endpoint | Description |
|---|---|---|
| GET | `/booking` | Get all bookings |
| GET | `/booking/:id` | Get booking by ID |
| GET | `/booking?firstname=` | Filter by first name |
| GET | `/booking?checkin=` | Filter by check-in date |
| POST | `/auth` | Generate auth token |
| POST | `/booking` | Create new booking |
| PUT | `/booking/:id` | Full update booking |
| PATCH | `/booking/:id` | Partial update booking |
| DELETE | `/booking/:id` | Delete booking |

---

## Test Types Covered

- ✅ Positive testing
- ✅ Negative testing
- ✅ Status code validation — 200, 201, 404, 403, 500
- ✅ Response body validation
- ✅ Response time validation
- ✅ Authentication testing
- ✅ Security testing — unauthorized access rejection
- ✅ Full CRUD coverage — GET, POST, PUT, PATCH, DELETE

---

## Environment Setup

Create a Postman environment with these variables:

| Variable | Value |
|---|---|
| `base_url` | `https://restful-booker.herokuapp.com` |
| `token` | *(auto-populated by TC-002)* |
| `booking_id` | *(auto-populated by TC-004)* |
| `new_booking_id` | *(auto-populated by TC-009)* |

---

## How to Run

1. Import `RestfulBooker_Hotel_API_Test_Suite.postman_collection.json` into Postman
2. Create environment with variables listed above
3. Select environment from top right dropdown
4. Right click collection → **Run Collection**
5. Click **Run** — all 53 assertions pass

---

## Author

**Abdul Hannan** — SQA Engineer
GitHub: [@AbdulHannan46](https://github.com/AbdulHannan46)

---

## License
MIT License
