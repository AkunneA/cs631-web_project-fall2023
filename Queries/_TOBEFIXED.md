Foreign key(s) on the following tables don't have on update/on delete actions specified:
* STATEPROV
* PATIENT
* PATIENT_SUGAR
* NDC
* SALARY
* NURSE_SKILL
* SURGEON_CONTRACT
* NURSE_EXP
* OWNER
* OWNERSHIP
* OP_THEATRE
* ROOM
* MED_INTERACT
* PRESCRIPTION
* PATIENT_ALLERGY
* PATIENT_ILLNESS
* SURG_TYPE
* SURG_TYPE_SKILL
* INPATIENT_STAY
* SURGERY
* SURGERY_STAFF

Foreign key constraints need to be set up for the following tables/columns:
* PATIENT (Pcp, InsProvider)

The following tables have no sample data inserted yet:
* PATIENT_SUGAR
* NDC
* SALARY
* NURSE_SKILL
* SURGEON_CONTRACT
* SURG_PHYS_SPECIALTY
* NURSE_EXP
* MED_INTERACT
* PRESCRIPTION
* PATIENT_ALLERGY
* PATIENT_ILLNESS
* SURG_TYPE
* SURG_TYPE_SKILL
* INPATIENT_STAY
* SURGERY
* SURGERY_STAFF

The following tables may need to be split up into multiple:
* NDC