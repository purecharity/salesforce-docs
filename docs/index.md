# Salesforce Pure Charity App Documentation

This repository contains some relevant information on how the Pure Charity App for Salesforce works and how the information will be mapped there.

The latest version available can always be found [here](http://salesforceinstall.purecharity.com).

You can also all take a look at the [Changelog file](changelog.md) and see what changed from version to version.

## Installation
In order to integrate Pure Charity with your Salesforce instance, please follow these steps:

1. Make sure that the Nonprofit Starter Pack is installed in your Salesforce account [NPSP3 Installer page](https://mrbelvedere.salesforcefoundation.org/mpinstaller/npsp).

2. Create or designate an Integration user in your Salesforce instance. This user must be a system admin with "Marketing User" activated and must have permissions to create and edit donations.

3. Install the Pure Charity App into your Salesforce account [Salesforce.com install page](http://salesforceinstall.purecharity.com).

4. Once the Pure Charity App is installed, please click the authorize button on the Salesforce section of your Pure Charity dashboard to initiate the integration process.


## Mapping

The integration will take care to send the following information to Salesforce:

- [Donations](mapping/donations.md)
- [Direct donations](mapping/direct_donations.md)
- [Direct donations to specific categories](mapping/donation_categories.md)
- [Fundraisers](mapping/fundraisers.md)
- [Sponsorships Programs](mapping/sponsorship_programs.md)
- [Sponsorships](mapping/sponsorships.md)
- [Trips](mapping/trips.md)
- [Trip Registrations](mapping/registrations.md)
- [Users](mapping/users.md)
- [Mission passport](mapping/mission_passport.md)
- [Giving Circles](mapping/giving_circles.md)
- [Adjustments](mapping/adjustments.md)
