# Donation Categories

Every Donation Category created have a Campaign as well to address direction donation following the mapping bellow.

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Name | `Name` | Text (80) | Donation Category name
Active | `IsActive` | Checkbox | `true`
Type | `Type` | Picklist | "Direct Donation"
Status | `Status` | Picklist | "In Progress"
Parent Campaign | `Parent` | Lookup(Campaign) | Field Partner's Direct Donation Campaign
Campaign Record Type | `RecordType` | Record Type | Pure Charity Direct Donation (`Pure_Charity_Direct_Donation`)
Pure Charity URL | `purecharity__Url__c` | URL(255) | Pure Charity URL address to the Field Partner profile
Pure Charity Reference | `purecharity__Reference__c` | Text(255) | Field Partner Reference Code
Contact | `purecharity__Contact__r` | Lookup(Contact) | Field Partner Organizer Contact
Organizer | `purecharity__Organizer__r` | Lookup(Account) | Field Partner Organizer Account
