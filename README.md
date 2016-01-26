# politwoops-data

Storage for data associated with politwoops.

## Files in this repository

### accounts.csv

Contains the curated list of politicians for which we wish to track deleted tweets. The fields for the CSV are across the top and should be self explanatory aside from the **Linked Accounts** field. This field allows for Twitter handlers for different purposes (Official, Campaign, Personal, etc) to be related together by putting each related handler separated by a | character. For instance, if John Doe has three twitter handlers (`johndoe55`, `DoePress`, `DoeHouseRep`) then the row entry for `johndoe55` would contain `DoePress|DoeHousRep` in the Linked Accounts field, the row entry for `DoePress` would contain `johndoe55|DoeHouseRep` in the Linked Accounts field, and the row entry for `DoeHouseRep` would contain `johndoe55|DoePress` in the Linked Accounts field. Look for examples in the existing data if this is unclear. It is not required that these entries be sequential but it would make maintaining the record easier.
