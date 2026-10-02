# Non-Functional & Security Requirements

Source: HMS SRS v1.0.

## Performance
- **NFR-PERF-01:** The system shall process queries and display results within 2 seconds for a database of up to 10,000 records.
- **NFR-PERF-02:** The system footprint shall not exceed 50 MB in RAM during normal operations.

## Reliability & Availability
- **NFR-REL-01:** The system shall prevent data corruption in the event of an abrupt application crash (ACID compliance via SQLite).
- **NFR-REL-02:** The application shall handle missing data files gracefully by creating necessary empty files on startup.

## Security
- **SEC-REQ-01:** Passwords shall not be stored in plain text (must be hashed, e.g., SHA-256).
- **SEC-REQ-02:** The system shall use parameterized queries for all SQLite interactions to prevent SQL Injection.
- **SEC-REQ-03:** Role-based access checks shall occur server/backend-side before executing any sensitive operation.

## Maintainability
- **NFR-MAINT-01:** The source code shall be documented using Doxygen-style comments.
- **NFR-MAINT-02:** Memory leaks shall be verified as zero using Valgrind before release.
