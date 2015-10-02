# Sponsorships

When a Sponsorship is created in the Pure Charity platform a Campaign will be created in the Salesforce instance as well following the mapping bellow.

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Name | `Name` | Text (80) | A combination of Sponsorship Program Name, Sponsorship name and Sponsorship reference separated by dashes (i.e.: "Program - John Doe - SPOREF1234")
Sponsorship Name | `purecharity__SponsorshipName__c` | Text (255) | Sponsorship name
Active | `IsActive` | Checkbox | `true`
Type | `Type` | Picklist | "Sponsorship"
Status | `Status` | Picklist | "In Progress"
Expected Revenue | `ExpectedRevenue` | Currency(18, 0) | Sponsorship funding goal
Parent Campaign | `Parent` | Lookup(Campaign) | Sponsorship Program Campaign
Campaign Record Type | `RecordType` | Record Type | Pure Charity Sponsorship (`Pure_Charity_Sponsorship`)
Region of Impact | `purecharity__Region__c` | Text(255) | Sponsorship region of impact
Pure Charity URL | `purecharity__Url__c` | URL(255) | Pure Charity's URL address to the Sponsorship
City/Country of Impact | `purecharity__Location__c` | Text(255) | Sponsorship location of impact
Contact | `purecharity__Contact__r` | Lookup(Contact) | Sponsorship Organizer Contact (Admin or Owner)
Organizer | `purecharity__Organizer__r` | Lookup(Account) | Sponsorship Organizer Account (Admin or Owner)
