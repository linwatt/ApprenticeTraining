1) Basic app that does addition, multiplication, subtraction and division
2) Code should be uploaded to github
3) Code should be developed in Android Studio
4) Use Emulator for manual GUI testing
5) Create unit tests for command line testing

<h2>User Story</h2>
**A user can enter a math equation and see the solution**
As a User
I want to be able to enter 2 numbers 
And select a math operation
So that I can see the solution to the equation I entered

<h2>Acceptance Criteria</h2>
**A user can only enter numbers**
Given I am a user
When I enter something other than a number
Then I receive an error message

**A user can enter a math operation**
Given I have entered the first number
When I press a button for addition/subtraction/multiplication/division
Then I see that symbol added to the equation

**Pressing 'equals' shows the solution**
Given I have entered a number, an operation and a second number
When I press 'equals'
Then I can see the answer to the math equation

**A user can press 'clear' to enter another math equation**
Given I have entered a math equation
When I press 'clear'
Then I am able to enter another math equation