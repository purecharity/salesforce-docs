# Users

Pure Charity Users will only be created in Salesforce when they donate to any of Field Partner's campaigns inside Pure Charity platform.

Not necessarily all user's personal information will be sent to Salesforce. The user can opt to not share his information with any Field Partners.

For any User, a Account and a Contact will be created in the Salesforce instance following the mapping bellow.

## Account

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Account Name | `Name` | Name | User's name
Type | `Type` | Picklist | "Backer"
Phone | `Phone` | Phone | User's phone (if allowed)
Billing Address | `BillingAddress` | Address | User's address (if allowed)
Pure Charity URL | `purecharity__Url__c` | URL(255) | URL address to the User's profile on Pure Charity
Lives Impacted | `purecharity__LivesImpacted__c` | Number(18, 0) | Number of lives impacted by the User on Pure Charity (if allowed)
Email | `purecharity__Email__c` | Email | User's Email (if allowed)

## Contact

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
First Name | `FirstName` | Text(40) | User's first name
Last Name | `LastName` | Text(80) | User's last name
Salutation | `Salutation` | Picklist | User's salutation (if allowed)
Email | `Email` | Email | User's email (if allowed)
Phone | `Phone` | Phone | User's phone (if allowed)
Mobile | `MobilePhone` | Phone | User's mobile phone (if allowed)
Birthdate | `Birthdate` | Date | User's birthdate (if allowed)
Mailing Address | `MailingAddress` | Address | User's address (if allowed)
Account Name | `Account` | Lookup(Account) | User's account
Donor Reference | `purecharity__DonorReference__c` | Text(255) | User reference code

## Mission Passport

Additionally the integration can send data from the standard forms submitted by the trip participants. For more information you can check the [mission passport mapping](mission_passport.md).
