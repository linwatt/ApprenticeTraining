Key Points
1) Store list of tasks in SQLite database
2) Use MVP design pattern using Dagger
3) Create JUnit4 tests using Robolectric
4) Mock out the database

Something like
https://github.com/avjinder/Minimal-Todo

<h2>User Stories</h2>
**A User can enter a to-do item**
As a user
I want to be able to enter a to-do item
So that I can keep track of what I need to do

**Acceptance Criteria**
**The app opens to a list of to-do items**
Given I am a user
When I open the app
Then I am on a screen that shows a list of to-do items

**A user can view a form to add a new to-do item**
Given I am on the main screen
When I press the 'add' button
Then I can view a form for adding a new to-do item

**A user must enter a name for a to-do item**
Given I am viewing the form for adding a new to-do item
When I do not enter a name for the item
And I press 'save'
Then I receive an error message

Given I am viewing the form for adding a new to-do item
When I enter a name for the item
And i press 'save'
Then the item is saved
And I am taken back to the main to-do list screen

**New to-do items show on the main to-do list screen**
Given I have added a new to-do item
When I am taken back to the main to-do screen
Then I can see the name of the item I saved in the list of to-dos

<h2></h2>
**A user can enter a completion date and time for a to-do**
As a user
I want to be able to enter a completion date and time for a to-do item
So that I can keep track of when my items are due

**Acceptance Criteria**
**A User can enter a completion date and time for a to-do item**
When I am viewing the form for adding a new to-do item
Then I can enter a completion date
And I can enter a completion time

**To-do items with a completion date or completion time are shown on the main to-do list**
Given I am viewing the form for adding a new item
And I enter a completion date
Or I enter a completion time
When I press 'save'
Then i am taken to the list showing all to-do items
And the item I entered is shown with the completion date and/or time as a sub item

<h2></h2>
**A user can edit a to-do item**
As a user
I want to be able to edit a to-do item
So that I can change the information

**A user can delete a to-do item**
As a user
I want to be able to delete a to-do item
So that I can remove it from my list of to-dos

**Acceptance Criteria**
**Pressing a to-do item from the main list opens the form for editing the details**
Given I am on the main list of to-do items
When I press the listing for a to-do item
Then I am taken to a screen showing the details of the to-do item with the fields pre-populated with the previously entered details
And I can edit the details

**Pressing 'save' will save the new details for the to-do item**
Given I am on the form for editing a to-do item
When I press 'save'
Then I am taken to the main list showing all to-do items
And I can see the to-do item with the updated details

**Pressing 'delete' for an item prompts the user to confirm**
Given I am on the form for editing a to-do item
When I press 'Delete'
Then I receive a prompt "Delete Item?"
With the options "Cancel" and "Delete"

Given I am viewing a prompt to delete an item
When I press "Delete"
Then I am taken back to the main list of to-do items
And the to-do is no longer listed

Given I am viewing a prompt to delete an item
When I press "Cancel"
Then I remain on the form for editing the details of the to-do item

<h2></h2>
**A user can mark a to-do item as completed**
As a user
I want to be able to mark a to-do item as completed
So that I can tell which to-dos I have left to complete

**Acceptance Criteria**
**A user can mark a to-do item as completed from the main list of to-dos**
Given I am on the main list of to-do items
When I press the checkbox next to a to-do item
Then the to-do item is marked as completed
And the to-do item is removed from the list


