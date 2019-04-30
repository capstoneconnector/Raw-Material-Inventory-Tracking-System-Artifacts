# Requirement Match Document
----
### Requirements
This document will list all of the requirements that were meant to be implementedin the project. In addition to this list, all requirements that were implemented will be separated from those that were not. 

##### Requirements Met:
- Adding, Updating, Removing Tracked Materials
- Adding, Updating, Removing Material Inventory
- Track Inventory Amounts
  - Initial Amount
  - Current Amount
  - Prepared Amount
- Track Inventory Expiration Date
   - Ordered by expiration date
   - Visible signifiers of expired materials
- Track User Activity
   - When changes were made
   - Who made the changes
   - What was changed

##### Requirements Not Met:
- Separating inventory based on a selected restaurant (Low Priority)
   - Adding multiple restaurant management was a low priority feature that was not implemented due to lack of time.
    To achieve this, one would have to add a Restaurant model that relates to Material types and Users. It is important to know only assigned employees of a specific restaurant can view and manage the inventory of their restaurant. 
- Mobile friendly (Medium Priority)
   - Mobile friendly interface was not achieved due to the change in front-end development tools. Originally, React JS was to be used in order to make for a mobile friendly and web browser friendly service. However, React JS was dropped and our views are rendered in HTML & CSS in order to implement more features in time. 
- Calculating Profit (Low Priority)
  - Also a low priority feature. It became less of a requirement and more of a possible additional feature. Calculating cost of an item would require more features to the Material Type model. One would have to take in account the cost per pound of an item and calculate profit based on the usage, removal, or adding of material inventory.  