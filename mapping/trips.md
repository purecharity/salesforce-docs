# Trips

When a Event/Trip is created in the Pure Charity platform a Campaign will be created in the Salesforce instance as well following the mapping bellow.

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Name | `Name` | Text (80) | Trip name
Active | `IsActive` | Checkbox | `true`
Type | `Type` | Picklist | "Trip"
Status | `Status` | Picklist | "In Progress"
Start Date | `StartDate` | Date | Trip start date
End Date | `EndDate` | Date | Trip end date
Campaign Record Type | `RecordType` | Record Type | Pure Charity Trip (`Pure_Charity_Trip`)
Region of Impact | `purecharity__Region__c` | Text(255) | Trip region of impact
Pure Charity URL | `purecharity__Url__c` | URL(255) | Pure Charity's URL address to the Trip
City/Country of Impact | `purecharity__Location__c` | Text(255) | Trip location of impact
Contact | `purecharity__Contact__r` | Lookup(Contact) | Trip Organizer Contact (Admin or Owner)
Organizer | `purecharity__Organizer__r` | Lookup(Account) | Trip Organizer Account (Admin or Owner)
