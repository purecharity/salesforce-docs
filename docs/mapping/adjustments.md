# Adjustments (Promotional Transfers)

When a promotional adjustment or transfer is made in the Pure Charity platform an Opportunity record will be created in the Salesforce instance following the mapping bellow.

## Opportunity

Label | API Name | Type | Description
--- | --- | --- | ---
Pure Charity ID | `purecharity__Id__c` | Text(255) (External ID) (Unique Case Sensitive) | Internal Pure Charity ID
Opportunity Name | `Name` | Text(120) | A combination of Source Campaign (if provided), Amount, Destination Campaign, Type and Close Date separated by a dash (i.e.: "Some Fundraiser - 300.00 - Another Fundraiser - Promotional Transfer - 2017-02-03")
Primary Campaign Source | `Campaign` | Lookup(Campaign) | Destination Campaign
Opportunity Record Type | `RecordType` | Record Type | "Pure Charity Adjustment"
Amount | `Amount` | Currency(16, 2) | Adjustment amount
Stage | `StageName` | Picklist | "Closed Won"
Close Date | `CloseDate` | Date | Adjustment date
Probability (%) | `Probability` | Percent(3, 0) | "100%"
Description | `Description` | Long Text Area(32000) | Adjustment description
Type | `Type` | Picklist | "Promotional Adjustment" or "Promotional Transfer"
Transfer Source | `purecharity__TransferSource__c` | Lookup(Campaign) | Source transfer campaign (if provided)
Donation Notes | `purecharity__Notes__c` | Long Text Area(32768) | Field Partner notes

