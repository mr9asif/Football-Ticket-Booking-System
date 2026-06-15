# ⚽ Football Ticket Booking System

A **Database Management System (DBMS)** assignment that demonstrates **database design**, **Entity Relationship Diagram (ERD)**, and **SQL queries** for a Football Ticket Booking System.

---

## 📖 Project Overview

This project manages:

* Football Fans and Ticket Managers
* Football Matches
* Ticket Bookings
* Payment Status
* Match Ticket Pricing

The project demonstrates various SQL concepts including filtering, joins, subqueries, aggregation, pattern matching, NULL handling, and pagination.

---

# 🗄️ Database Tables

## 1. Users

| Column       | Description                   |
| ------------ | ----------------------------- |
| user_id      | Primary Key                   |
| full_name    | User's full name              |
| email        | User email address            |
| role         | Football Fan / Ticket Manager |
| phone_number | Contact number                |

---

## 2. Matches

| Column              | Description        |
| ------------------- | ------------------ |
| match_id            | Primary Key        |
| fixture             | Teams playing      |
| tournament_category | Tournament name    |
| base_ticket_price   | Ticket price       |
| match_status        | Match availability |

---

## 3. Bookings

| Column         | Description           |
| -------------- | --------------------- |
| booking_id     | Primary Key           |
| user_id        | Foreign Key → Users   |
| match_id       | Foreign Key → Matches |
| seat_number    | Seat number           |
| payment_status | Payment status        |
| total_cost     | Total booking cost    |

---

# 🔗 Entity Relationship Diagram (ERD)

Relationship Summary:

* One User → Many Bookings
* One Match → Many Bookings
* Each Booking belongs to one User and one Match

## ERD Screenshot

```markdown
 <img width="1481" height="647" alt="ERD" src="https://github.com/user-attachments/assets/da1cb38e-86a2-4000-b2fd-b78fac6930c9" />

```

Or add your DrawSQL public link:

```text
[https://drawsql.app/teams/mr9asif/diagrams/football-ticket-booking-2]
```

---

# 📋 SQL Queries Implemented

### Query 1

Retrieve all available Champions League matches.

### Query 2

Find users whose names start with **Tanvir** or contain **Haque**.

### Query 3

Replace NULL payment status with **Action Required** using `COALESCE()`.

### Query 4

Retrieve booking details with user names and match fixtures using `INNER JOIN`.

### Query 5

Display all users including those without bookings using `LEFT JOIN`.

### Query 6

Find bookings where the total cost is greater than the average booking cost.

### Query 7

Retrieve the top two most expensive matches after skipping the highest-priced match using `LIMIT` and `OFFSET`.

---

# 💻 SQL Concepts Used

* SELECT
* WHERE
* LIKE
* ILIKE
* IS NULL
* COALESCE
* INNER JOIN
* LEFT JOIN
* PRIMARY KEY
* FOREIGN KEY
* Aggregate Functions (AVG)
* Subqueries
* ORDER BY
* LIMIT
* OFFSET

---

# 📂 Repository Structure

```text
Football-Ticket-Booking-System/
├── answer.sql
├──── README.md
├── ERD.png

```

---

# 🛠️ Technologies Used

* PostgreSQL
* SQL
* DrawSQL
* DB Fiddle
* Git & GitHub

---

# 👨‍💻 Author

**mr9asif**

Computer Science Student || PH Student

Database Management System (DBMS) Assignment 3
