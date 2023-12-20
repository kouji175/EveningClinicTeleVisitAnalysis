# EveningClinicTeleVisitAnalysis

Some time ago, for our evening clinic (visits after 5:30pm) we explored the idea of providing telephone visits as an alternative to a face-to-face visit to patients to improve service.  We felt that this would be a more convenient alternative for the patient to get their medical needs met without having to come in.  Attached is about 6 months worth of visits, which includes the telephone encounters.  After we implemented the program, we wanted to use the visit data to determine how to staff for the evening appointments and evaluate the effectiveness of the program. 

# Data Set: 
See dataset folder

# Data Processing Workflow:
- Data Inspection
- Data Validation
- Missing value imputation
- Normality and Variance Alignment Testing
- Feature Engineering

# Data Analyze
- multiple linear regression models
- Chi square
- Data Visulization

# Appointment Data – Data Dictionary

| Field             | Description |
|-------------------|-------------|
| **FACILITY**      | Abbreviation for where the appointment took place |
| **DEPARTMENT**    | Abbreviation for the department where the appointment took place |
| **PROVIDER_ID**   | Identifier for the Physician who saw or provided advice to the patient |
| **APPOINTMENT_DATE** | Date the appointment was scheduled to take place |
| **APPOINTMENT_TIME** | Time the appointment was scheduled to take place |
| **PATIENT_ID**    | Identifier for the Patient who had the scheduled appointment |
| **APPOINTMENT_TYPE** | Type of appointment that was scheduled. Only two values:<br>• Telephone Visit<br>• In-Person Visit |
| **BOOKING_DATE**  | Date the scheduled appointment was booked |
| **BOOKING_TIME**  | Time the scheduled appointment was booked |
| **SHOW_CODE**     | Indicator of whether the patient showed up for the appointment:<br>• N/P – Patient did not show up for the scheduled appointment; Note – Check-In Date and Check-In Time will be null<br>• Y – Patient appeared for the scheduled appointment |
| **CHECKIN_DATE**  | Date the patient was registered for the appointment |
| **CHECKIN_TIME**  | Time the patient was registered for the appointment |

# Questions
* **How many physicians would you need to staff the after-hours (appointments after 5:30pm) telephone clinic?**
  * Assume that 1 physician can see 4 telephone visits per hour.

* **How effective are the Telephone Appointments during after-hours (appointments after 5:30pm)?**
  * An effective telephone appointment is one where there are no follow-up appointments to the call within the following 7 days.

* **Based on the available data, what suggestions would you have to improve the effectiveness of the telephone appointments (reduce the number of telephone appointments needing a follow-up appointment within 7 days)?**
  1. Explore providers who have a high effective ratio of after-hours telephone visits and providers who have a low effective ratio.
  2. Staffing 3-4 physicians after hours may be a better choice, as 3-4 physicians have shown a high effective ratio after hours.
  3. Pay attention to the efficiency rates of doctors, noting that it is generally higher on Mondays than other working days. This could suggest that after sufficient rest, doctors are more energized and effective in conducting telephone interviews.
  4. Investigate reasons why the effective ratio does not improve after 20:00, and consider actions to make physicians more careful and energized.


