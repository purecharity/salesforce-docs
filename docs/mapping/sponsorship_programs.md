# Sponsorship Programs

When a Sponsorship Program is created in the Pure Charity platform a Campaign will be created in the Salesforce instance as well following the mapping bellow.

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Name | `Name` | Text (80) | Sponsorship Program name
Active | `IsActive` | Checkbox | `true`
Type | `Type` | Picklist | "Sponsorship Program"
Status | `Status` | Picklist | "In Progress"
Expected Revenue | `ExpectedRevenue` | Currency(18, 0) | Sponsorship Program total goal
Parent Campaign | `Parent` | Lookup(Campaign) | Parent Campaign on Pure Charity
Campaign Record Type | `RecordType` | Record Type | Pure Charity Sponsorship Program (`Pure_Charity_Sponsorship_Program`)
Pure Charity URL | `purecharity__Url__c` | URL(255) | Pure Charity's URL address to the Sponsorship Program
Pure Charity Reference | `purecharity__Reference__c` | Text(255) | Sponsorship Program Reference Code
Contact | `purecharity__Contact__r` | Lookup(Contact) | Sponsorship Program Organizer Contact (Admin or Owner)
Organizer | `purecharity__Organizer__r` | Lookup(Account) | Sponsorship Program Organizer Account (Admin or Owner)
