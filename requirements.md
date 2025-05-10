# Airbnb Clone Backend Requirements

## 📌 User Authentication

**API Endpoints**
- `POST /api/register`
- `POST /api/login`
- `GET /api/user/:id`

**Validation Rules**
- Unique email
- Password minimum 8 characters
- Valid OAuth tokens for social login

**Performance Criteria**
- Response time < 500ms
- 99.5% authentication success rate

---

## 📌 Property Management

**API Endpoints**
- `POST /api/properties`
- `GET /api/properties`
- `GET /api/properties/:id`
- `PUT /api/properties/:id`
- `DELETE /api/properties/:id`

**Validation Rules**
- Required fields: title, description, location, price
- Image upload validation (file size/type)

**Performance Criteria**
- Search response time < 1s
- Listing creation < 800ms

---

## 📌 Booking System

**API Endpoints**
- `POST /api/bookings`
- `GET /api/bookings`
- `GET /api/bookings/:id`
- `DELETE /api/bookings/:id`

**Validation Rules**
- No overlapping bookings
- Valid property and user IDs
- Date validation (check-in before check-out)

**Performance Criteria**
- Booking response time < 1s
- Cancellation processing < 1s
