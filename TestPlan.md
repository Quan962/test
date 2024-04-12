# Test Plan

*This is the template for your test plan. The parts in italics are concise explanations of what should go in the corresponding sections and should not appear in the final document.*

**Author**: \<Quanxin Yu\>

## 1 Testing Strategy

### 1.1 Overall strategy

- I first go through the method functions used throughout the application and distinguish which ones are used by the user and which ones are used by the system. Then each given method will be a unique test plan,

### 1.2 Test Selection

- I will use the black-box technique because I think all the functions in the code detail have not been implemented yet, so based on the requirements, and expected behavior, I will create the test csae for the user using the function.

### 1.3 Adequacy Criterion

- Functionally, I aim to ensure that all user stories and requirements are adequately tested.

### 1.4 Bug Tracking

- each bug and enhancement request will have an issue tracking system to record, and each problem will have its unique identifier and be prioritized, then we will fix the problem by the prioritized lever. this activity will tracked throughout its lifecycle until resolution.

### 1.5 Technology

- I will use JUnit to create the test case for the user functions.

## 2 Test Cases



| Test Case ID | Function| Purpose| Steps| Expected Result | Actual Result | Pass/Fail | Additional Information  |
|----|---------|---------|-------------------------------|----------------|--------|---------|---------|
| 001 | additem(item: CheckListItem) | Add item to list from hierarchical UI | 1. Navigate to the hierarchical UI.<br /> 2. Select an item type.<br /> 3. Select a specific item.<br /> 4. Specify quantity.<br /> 5. Add this item with quantity and type. | The item should be added to the list with the specified quantity. |    as5     |   as5   | 5sa |
| 002 | Search(name: string) | Search for an item by typing its name | 1. Use search mode.<br /> 2. Type the item’s name.<br /> 3. Select the item.<br /> 4. Specify quantity.<br /> 5. Add it to a list. | The item should be added to the list with the specified quantity.                  |       as        |   as   |asas|
| 003 | Search(name: string) | Search for an item by typing its name but not find this item | 1. Use search mode.<br /> 2. Type the item’s name.<br /> 3. See if no item match with the search.<br /> 4. Return to the hierarchical level and ask user to select a type. | Go to hierarchical level UI to add a type, then use additem function.     |        |           |              |
| 004 | Check(item: CheckListItem, isChecked: boolean) | The check box of the item that can be checked  | 1. Navigate to an item.<br /> 2. Click on the box.<br />  | If the box is checked, it should turn to unchecked (false). If it is unchecked, it should turn to checked (true). |               |           |       |
| 005 | delete(item: CheckListItem)   | Delete an item from a list  | 1. Navigate to a list.<br /> 2. Select an item from this list.<br /> 3. Click “delete”.   | The item should be deleted from this list, and others should not be affected.       |    |           |    |
| 006 | create(name:string)| Create a new list  | 1. Select the create function.<br /> 2. Type a name to the list.<br /> | A new list with the name should be created.  |   |           |             |
| 007  | rename(oldName:string, newName:string)| Rename the list from the old name to the new name. | 1. Navigate to the list manager.<br /> 2. Use rename.<br /> 3. Type the old name of a list and the new name.  | The old name of the list will change to the new name.    |               |           |                |
| 008 | delete(name:string)| Delete the list with the name typed  | 1. Navigate to the list manager.<br /> 2. Use delete function.<br /> 3. Type the name want to delete. 4. Click delete.| The list will be deleted, and the items on the list will also be deleted.           |               |           |               |
| 009 | getGroceryList(name: String) | Display the list with the items on the list  | 1. Navigate to the list manager.<br /> 2. Use getGroceryList function. <br />3. Type the name of the list.  | Return the list we want and what items are on this list. |               |           |                         |
| 010  | getGroceryList(name: String) | If not found the list.| 1. Navigate to the list manager.<br /> 2. Use getGroceryList function.<br /> 3. Type the name of that not in the list. | Return error, can’t find the list.|               |           |        |
| 011  | CheckAll(checkall: boolean)| Clear all check-off marks in a list | 1. Navigate to the list.<br /> 2. Find the option to clear check-off marks.<br /> 3. Click on the option. | All check-off marks in the list should be cleared.   |               |           |                   |


