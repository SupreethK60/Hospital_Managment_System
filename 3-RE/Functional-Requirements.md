# Functional Requirements (FR)

Source: HMS SRS v1.0.

## Authentication & Authorization
- **FR-AUTH-01:** The system shall allow users to log in using a unique username and password.
- **FR-AUTH-02:** The system shall support three distinct roles: Admin, Receptionist, and Doctor.
- **FR-AUTH-03:** The system shall deny access to unauthorized users after three incorrect login attempts.
- **FR-AUTH-04:** The system shall enforce session termination upon explicit user logout.

## Patient Management
- **FR-PAT-01:** The system shall allow Receptionists to register a new patient with Name, Age, Gender, Contact, and Blood Group.
- **FR-PAT-02:** The system shall generate a unique alphanumeric Patient ID upon successful registration.
- **FR-PAT-03:** The system shall allow Receptionists and Doctors to search for a patient by Patient ID or Name.
- **FR-PAT-04:** The system shall allow Receptionists to update patient contact details.

## Doctor Management
- **FR-DOC-01:** The system shall allow Admins to add new doctors with Name, Specialization, and Contact Info.
- **FR-DOC-02:** The system shall generate a unique Doctor ID upon registration.
- **FR-DOC-03:** The system shall allow Admins to configure a doctor's weekly available hours.
- **FR-DOC-04:** The system shall allow Receptionists to view a list of all doctors filtered by Specialization.

## Appointment Management
- **FR-APP-01:** The system shall allow Receptionists to book an appointment by providing Patient ID, Doctor ID, Date, and Time.
- **FR-APP-02:** The system shall reject appointment bookings if the doctor is unavailable or already booked for the specified time.
- **FR-APP-03:** The system shall allow Receptionists to cancel an existing appointment using the Appointment ID.
- **FR-APP-04:** The system shall allow Receptionists to reschedule an appointment, subject to doctor availability.
- **FR-APP-05:** The system shall allow Doctors to view their scheduled appointments for a specific date.

## Reporting
- **FR-REP-01:** The system shall allow Admins to generate a daily report of total appointments booked, canceled, and completed.
- **FR-REP-02:** The system shall allow Admins to generate a report of all registered patients.
- **FR-REP-03:** The system shall export reports as basic text/CSV files to the local disk.
