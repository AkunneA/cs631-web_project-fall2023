[Back to Assignment Phases](0-AssignmentPhases.md)

# Database Design Requirements

Newark Medical Associates (MMA) is a clinic located in Newark, New Jersey, owned by a group 
of medical corporations and individual physicians. Clinic personnel include physicians, surgeons, 
nurses, and support staff. All clinic personnel except the surgeons are on an annual salary. 
Surgeons do not receive a salary but work for Newark Medical Associates on a contract basis. It 
is possible for a physician to have an ownership position in the clinic.

Since surgeons perform surgery on patients as needed, it is required that a surgery schedule 
keep track of the operation theatre where a surgeon performs a certain surgery type on a 
particular patient and when that surgery type is performed. Some patients need surgeries and 
others don’t. Surgeons perform surgeries in the clinic; some do a lot, and others just a few. 
Some surgery types are so rare that they may not yet have been performed in the clinic; but 
there are others that are performed numerous times. In addition, there is the need to keep 
track of nurses who can be assigned to a specific surgeon type since all nurses cannot be 
assigned to assist in all types of surgeries. A nurse cannot be assigned to more than one surgery 
type. It is the policy of the clinic that all types of surgery have at least two nurses. The clinic 
maintains a list of surgery skills. A surgery type requires at least one but often many surgery 
skills are utilized in numerous surgery types. However, all surgery skills are not utilized in the 
clinic while some surgery skills some surgery skills rate utilized in numerous surgery skills for 
which no nurse in the clinic qualifies; at the same there are certain surgery skills for which no 
nurse in the clinic qualifies; at the same time there are other surgery skills that have several 
qualified nurses. In order to assign a nurse to a surgery type, a nurse should possess one or 
more of the skills required for the surgery type.

Depending on the illness, some patients may stay in the clinic for a few days; but most require 
no hospitalization. In-patients are assigned a room and a bed. A nurse attends to several inpatients, but must have at least five. No more than one nurse attends to an inpatient; but some 
in-patients may not have any nurse attending to them. If a nurse leaves the clinic, temporarily 
remove the association of all in-patients previously attended to by that nurse in order to allow 
these patients to be transferred to another nurse at a later time. Every physician serves as a 
primary care physician for a least seven patients, however, no more than 20 patients are 
allotted to a physician... If a physician leaves the clinic, temporarily assign the physician’s 
patients to the clinic’s chief of staff. Clinic personnel can also become ill and be treated in the 
clinic. A patient is assigned one physician for primary care.

A patient may have several illnesses and several patients may have the same illness. In order to 
qualify as a patient, a patient must have a least one illness. Also, a patient may have several 
allergies that are also recorded. In order for a patient to be diagnosed with a disease or an 
allergy, the patient requests an appointment to see a doctor. The term used for these 
appointments is consultation. A patient sees most of the time his/her primary doctor but can 
also be consulted by other doctors. 

Physicians prescribe medications to patients; thus it is necessary to capture which physician(s) 
prescribes what medication(s) to which patient(s) along with dosage and frequency. In addition, 
no two physicians can prescribe the same medication to the same patient. If a physician leaves 
the clinic, all prescriptions prescribed by that physician should also be removed because this 
information is also retained in the archives. A person affiliated with the clinic as a surgeon 
cannot be deleted as long as a record of all surgeries performed by the surgeon is retained.

A patient may be taking several medications, and a particular medication may be taken by 
several patients. However, in order for a patient to take a medicine the medicine must be 
prescribed to that patient. As a medicine may interact with several other medicines, the 
severity of such interaction must be recorded in the system. Possible interactions include S = 
Severe interaction, M = Moderate interaction, L = Little interaction, and N = No interaction.

All clinic personnel have an employment number, name, gender (male or female), address and 
telephone number; with the exception of surgeons, all clinic personnel also have a salary (which 
can range from $25,000 to $300,000), but salaries of some can be missing. Each person who 
works in the clinic can be identified by an employment number. For each physician, his or her 
specialty is captured whereas for each surgeon data pertaining to his or her specialty and 
contract are captured. Contract data for surgeons include the type of contract and the length of 
the contract (in years). Grade and years of experience represent the specific data requirement 
for nurses.

A surgery code is used to identify each specific type of surgery. In addition the name category, 
anatomical location, and special needs are also captured for each surgery type. There are two 
surgery categories: those that require hospitalization (category= H) and those than can be 
performed on an outpatient basis (category = 0). A surgery skill is identified by its description 
and a unique skill code. Data for patients consists of personal data and medical data. Personal 
data includes patient number (the unique identifier of a patient), name, gender (male or 
female), date of birth, address, and telephone number. Medical data include the patient’s 
blood type, cholesterol (consisting of HDL, LDL, and triglyceride), blood sugar, and the code and 
name of all the patient’s allergies.

For both clinic personnel and patients, a Social Security number is collected. For each illness, a 
code and description are recorded. Additional data for each in-patient consists of a required 
data of admission along with the patient’s location (nursing unit, room number, and bed 
number). Nursing units a renumbered 1 through 7, rooms are located in either the Blue or 
Green wing , and the bed numbers in a room are labeled A or B. Medications are identified by 
their unique medication code and also include name, quantity on hand quantify on order, unit 
cost, and year to date usage. For medical corporations with ownership interest in the clinic the 
corporation name and headquarters are obtained. Corporation name uniquely identifies a 
medical corporation. The percentage ownership of each clinic is also recorded. 

The physicians who work in the clinic have recently embarked on a program to monitor the 
cholesterol level of its patients because cholesterol contributes to heart disease. Risk of heart 
disease is classified as N (None), L (Low), M (Moderate), and H (High). The ratio of the person’s 
total cholesterol divided by HDL is used in the field of medicine as one indicator of heart risk. 
Total cholesterol is calculated as the sum the HDL, LDL, and one fifth of triglycerides. A total 
cholesterol/HDL, ratio less than 4 suggests no risk of heart disease due to cholesterol, a ratio 
between 4 and 5 reflects a low risk, and a ratio greater than 5 is moderate risk. The high risk 
category is not coded as a function of cholesterol.