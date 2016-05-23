# Giving Circles

Pure Charity Giving Circles will only be created in Salesforce when they donate to any of Field Partner's campaigns inside Pure Charity platform.

For any Giving Circle, a Account will be created and the Giving Circle's Public Organizer will have a ContactRole associated with the Giving Circle in the Salesforce instance following the mapping bellow.

The Giving Circle's Public Organizer will be added as following the [Users](users.md) mapping as well.

## Account

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Account Name | `Name` | Name | Giving Circle's name
Type | `Type` | Picklist | "Giving Circle"
Phone | `Phone` | Phone | Public Organizer's phone
Billing Address | `BillingAddress` | Address | Public Organizer's address
Pure Charity URL | `purecharity__Url__c` | URL(255) | URL address to the Giving Circle's profile on Pure Charity
Lives Impacted | `purecharity__LivesImpacted__c` | Number(18, 0) | Number of lives impacted by the Giving Circle on Pure Charity
Email | `purecharity__Email__c` | Email | Public Organizer's Email

## ContactRole

Label | API Name | Type | Description
--- | --- | --- | ---
Contact | `Contact` | Lookup(Contact) | Public Organizer's Contact
Account | `Account` | Lookup(Account) | Giving Circle's Account
Primary | `IsPrimary` | Checkbox | `true`
