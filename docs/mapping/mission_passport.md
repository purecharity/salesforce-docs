# Mission Passport

Mission passport information is sent to Salesforce when any of the participant's requirement is approved and completed inside Pure Charity platform. All mission passport fields are sent to the participant's Contact.

Currently the integration sends only data for the following Standard Forms: Personal Information, Business Affiliation, Church Affiliation, Family Information, Emergency Contact, Medical, Passport and Skills.

**NOTE: Mission passport fields are not added by the Pure Charity App, they are all optional and should be added to the `Contact` object following the mapping bellow.**

## Contact

__Personal Information__

API Name | Type | Description
--- | --- | ---
`FirstName` | Text | First Name field
`MiddleName` | Text | Middle Name field
`LastName` | Text | Last Name field
`purecharity_pi_PreferredName__c` | Text | Preferred Name field
`Email` | Text | Email field
`Phone` | Text / Phone | Home Phone field
`MobilePhone` | Text / Phone | Mobile Phone field
`Birthdate` | Date | Birthdate field
`MailingCity` | Text | City field
`MailingCountry` | Text / Picklist | Country field
`MailingPostalCode` | Text | Zip field
`MailingState` | Text / Picklist | State field
`MailingStreet` | Text | Street Address + Apt/Suite field
`purecharity_pi_Gender__c` | Text / Picklist | Gender field
`Suffix` | Text / Picklist | Suffix field
`Salutation` | Text / Picklist | Tittle field
`purecharity_pi_ShirtSize__c` | Text / Picklist | Shirt Size field
`purecharity_pi_TripSource__c` | Text / Picklist | Trip Source field

__Family Information__

API Name | Type | Description
--- | --- | ---
`purecharity_fi_MaritalStatus__c` | Text / Picklist | Marital Status field

__Business Affiliation__

API Name | Type | Description
--- | --- | ---
`purecharity_ca_BusinessName__c` | Text | Business Name field
`purecharity_ca_BusinessAddress1__c` | Text | Business Address 1 field
`purecharity_ca_BusinessAddress2__c` | Text | Business Address 2 field
`purecharity_ca_BusinessCity__c` | Text | Business City field
`purecharity_ca_BusinessState__c` | Text / Picklist | Business State field
`purecharity_ca_BusinessZip__c` | Text | Business Zip field
`purecharity_ca_BusinessPosition__c` | Text | Business Position field
`purecharity_ca_BusinessProfession__c` | Text | Business Profession field
`purecharity_ca_BusinessPhone__c` | Text / Phone | Business Phone field

__Church Affiliation__

API Name | Type | Description
--- | --- | ---
`purecharity_ca_ChurchName__c` | Text | Church Name field
`purecharity_ca_ChurchAddress__c` | Text | Church Address field
`purecharity_ca_ChurchCity__c` | Text | Church City field
`purecharity_ca_ChurchState__c` | Text / Picklist | Church State field
`purecharity_ca_ChurchZip__c` | Text | Church Zip field
`purecharity_ca_ChurchPhone__c` | Text / Phone | Church Phone field
`purecharity_ca_PastorFirstName__c` | Text | Church's Pastor First Name field
`purecharity_ca_PastorLastName__c` | Text | Church's Pastor Last Name field
`purecharity_ca_PastorPhone__c` | Text / Phone | Church's Pastor Phone field
`purecharity_ca_PastorEmail__c` | Text | Church's Pastor Email field

__Emergency Contact__

API Name | Type | Description
--- | --- | ---
`purecharity_ec1_FirstName__c` | Text | Emergency Contact #1 First Name field
`purecharity_ec1_LastName__c` | Text | Emergency Contact #1 Last Name field
`purecharity_ec1_Address__c` | Text | Emergency Contact #1 Address field
`purecharity_ec1_City__c` | Text | Emergency Contact #1 City field
`purecharity_ec1_State__c` | Text / Picklist | Emergency Contact #1 State field
`purecharity_ec1_Zip__c` | Text | Emergency Contact #1 Zip field
`purecharity_ec1_Email__c` | Text | Emergency Contact #1 Email field
`purecharity_ec1_HomePhone__c` | Text / Phone | Emergency Contact #1 Home Phone field
`purecharity_ec1_MobilePhone__c` | Text / Phone | Emergency Contact #1 Mobile Phone field
`purecharity_ec1_Relation__c` | Text / Picklist | Emergency Contact #1 Relation field
`purecharity_ec2_FirstName__c` | Text | Emergency Contact #2 First Name field
`purecharity_ec2_LastName__c` | Text | Emergency Contact #2 Last Name field
`purecharity_ec2_Address__c` | Text | Emergency Contact #2 Address field
`purecharity_ec2_City__c` | Text | Emergency Contact #2 City field
`purecharity_ec2_State__c` | Text / Picklist | Emergency Contact #2 State field
`purecharity_ec2_Zip__c` | Text | Emergency Contact #2 Zip field
`purecharity_ec2_Email__c` | Text | Emergency Contact #2 Email field
`purecharity_ec2_HomePhone__c` | Text / Phone | Emergency Contact #2 Home Phone field
`purecharity_ec2_MobilePhone__c` | Text / Phone | Emergency Contact #2 Mobile Phone field
`purecharity_ec2_Relation__c` | Text / Picklist | Emergency Contact #2 Relation field

__Medical__

API Name | Type | Description
--- | --- | ---
`purecharity_me_Allergies__c` | Text | Allergies field
`purecharity_me_BloodType__c` | Text / Picklist | Blood Type field
`purecharity_me_HealthProblems__c` | TextArea | Health Problems field
`purecharity_me_Medications__c` | TextArea | Medications field
`purecharity_me_SleepProblems__c` | TextArea | Sleep Problems field

__Passport__

API Name | Type | Description
--- | --- | ---
`purecharity_pa_Birthplace__c` | Text | Birthplace field
`purecharity_pa_PassportCountry__c` | Text | Passport Country field
`purecharity_pa_PassportExpires__c` | Date | Passport Expires field
`purecharity_pa_PassportIssueDate__c` | Date | Passport Issue Date field
`purecharity_pa_PassportIssuePlace__c` | Text | Passport Issued From field
`purecharity_pa_PassportNumber__c` | Text | Passport Number field
`purecharity_pa_DepertureAirport__c` | Text | Departure Airport field

__Skills__

API Name | Type | Description
--- | --- | ---
`purecharity_sk_LanguageProficiency__c` | Text / Picklist | Language Proficiency field
`purecharity_sk_Language__c` | Text | Language field
`purecharity_sk_OtherSkills__c` | Text | List Other Skills field
`purecharity_sk_PastorPreacher__c` | Text / Picklist | Are you a pastor or preacher? field
`purecharity_sk_Sing__c` | Text / Picklist | Would you be willing to sing? field
`purecharity_sk_Speak__c` | Text / Picklist | Would you be willing to speak? field
