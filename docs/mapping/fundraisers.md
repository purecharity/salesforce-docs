# Fundraisers

When a Fundraiser is created in the Pure Charity platform a Campaign will be created in the Salesforce instance as well following the mapping bellow.

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Name | `Name` | Text (80) | Fundraiser name
Active | `IsActive` | Checkbox | `true`
Type | `Type` | Picklist | Campaign type on Pure Charity. Check the [Types](#types) table below for the available options
Status | `Status` | Picklist | "In Progress"
Start Date | `StartDate` | Date | Fundraiser start date
End Date | `EndDate` | Date | Fundraiser end date
Expected Revenue | `ExpectedRevenue` | Currency(18, 0) | Fundraiser funding goal
Parent Campaign | `Parent` | Lookup(Campaign) | Parent Campaign on Pure Charity
Campaign Record Type | `RecordType` | Record Type | Pure Charity Fundraiser (`Pure_Charity_Fundraiser`)
Organization Campaign ID | `purecharity__CampaignId__c` | Text(255) | Fundraiser Campaign ID
Organization Appeal ID | `purecharity__AppealId__c` | Text(255) | Fundraiser Appeal ID
Lives Impacted | `purecharity__LivesImpacted__c` | Number(18, 0) | Number of lives Impacted by the Fundraiser
Region of Impact | `purecharity__Region__c` | Text(255) | Fundraiser region of impact
Pure Charity URL | `purecharity__Url__c` | URL(255) | Pure Charity's URL address to the Fundraiser
City/Country of Impact | `purecharity__Location__c` | Text(255) | Fundraiser location of impact
Fundraiser Goal | `purecharity__FundraiserGoal__c` | Picklist | Campaign Goal type on Pure Charity. Check the [Goal Types](#goal-types) table below for the available options
Cause Category | `purecharity__CauseCategory__c` | Picklist | Campaign Category on Pure Charity. Check the [Cause Categories](#cause-categories) table below for the available options
Trip/Fund ID | `purecharity__TripId__c` | Text(255) | Fundraiser Trip/Fund ID
Pure Charity Reference | `purecharity__Reference__c` | Text(255) | Fundraiser Reference Code
Contact | `purecharity__Contact__r` | Lookup(Contact) | Fundraiser Organizer Contact (Admin or Owner)
Organizer | `purecharity__Organizer__r` | Lookup(Account) | Fundraiser Organizer Account (Admin or Owner)

## Types

Name | Description
--- | ---
Active Fundraiser | For Pure Charity's Race or Sport Activity Fundraisers
Adoption Fundraiser | For Pure Charity's Adoption Fundraisers
Birthday Fundraiser | For Pure Charity's Birthday Fundraisers
Get Creative Fundraiser | For Pure Charity's "Your fundraising idea" Fundraisers
Group Fundraiser | For Pure Charity's "With a Group" Fundraisers
Holiday Fundraiser | For Pure Charity's Holiday Fundraisers
Mission Fundraiser | For Pure Charity's Mission Trip Fundraisers
Occasion Fundraiser | For Pure Charity's Special Occasion Fundraisers


## Goal Types

| Name |
| --- |
| One-time |
| Monthly Recurring |
| One-time & Monthly Recurring |

## Cause Categories

| Name |
| --- |
| Water |
| Freedom |
| Food |
| Health |
| Relief |
| Opportunity |
