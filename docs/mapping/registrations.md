# Trip Registrations

When a trip registration is made in the Pure Charity platform a Campaign Member record will be created in the Salesforce instance following the mapping bellow.

## Campaign Member

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Contact | `Contact` | Lookup(Contact) | Pure Charity User Contact
Campaign | `Campaign` | Lookup(Campaign) | Pure Charity Campaign
Registration Type | `purecharity__RegistrationType__c` | Picklist | "Trip Leader" or "Participant"
Registration Status | `purecharity__RegistrationStatus__c` | Picklist | "Registered" or "Not Registered"
Registration Date | `purecharity__RegistrationDate__c` | Date | Registration date
Business Affiliation Completed | `purecharity__BusinessAffiliationCompleted__c` | Checkbox | Checked if the Business Affiliation todo is approved and completed.
Church Affiliation Completed | `purecharity__ChurchAffiliationCompleted__c` | Checkbox | Checked if the Church Affiliation todo is approved and completed.
Emergency Contact Completed | `purecharity__EmergencyContactCompleted__c` | Checkbox | Checked if the Emergency Contact todo is approved and completed.
Family Information Completed | `purecharity__FamilyInformationCompleted__c` | Checkbox | Checked if the Family Information todo is approved and completed.
Medical Completed | `purecharity__MedicalCompleted__c` | Checkbox | Checked if the Medical todo is approved and completed.
Passport Completed | `purecharity__PassportCompleted__c` | Checkbox | Checked if the Passport todo is approved and completed.
Personal Information Completed | `purecharity__PersonalInformationCompleted__c` | Checkbox | Checked if the Personal Information todo is approved and completed.
Personal Testimony Completed | `purecharity__PersonalTestimonyCompleted__c` | Checkbox | Checked if the Personal Testimony todo is approved and completed.
Skills Completed | `purecharity__SkillsCompleted__c` | Checkbox | Checked if the Skills todo is approved and completed.
