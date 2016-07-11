1) Basic app that does addition, multiplication, subtraction and division
2) Code should be uploaded to github
3) Code should be developed in Android Studio
4) Use Emulator for manual GUI testing
5) Create unit tests for command line testing

<h2>User Story</h2>
**A user can enter a math calculation and see the solution**
As a User
I want to be able to enter a calculation
So that I can see the solution to the calculation I entered

<h2>Acceptance Criteria</h2>
**A user can only enter numbers and decimals as values**
When I enter something other than a number or a decimal as a value
Then I receive an error message "Invalid character"

**A user can select a math operation**
Given I have entered the first value
When I press a button for addition/subtraction/multiplication/division
Then that operation is performed in the calculation

**A user cannot divide by zero**
Given I have selected division as the operation, and entered 0 as the divisor
When I press 'equals'
Then I receive an error message "Cannot divide by zero"

**Pressing 'equals' shows the solution**
Given I have entered a valid equation
When I press 'equals'
Then I can see the solution to the math equation

Given i have entered an invalid calculation 
(example: 3 -/ 4 ++ 7)
When I press 'equals'
Then I receive an error message "invalid calculation. check your values and try again"

**A solution can be a decimal**
Given I have entered a calculation that will result in a solution that is not an integer (example: 3 / 4)
When I press 'equals'
Then the solution is shown as the decimal value

**A user can press 'clear' to enter another math equation**
Given I have entered a math equation
When I press 'clear'
Then I am able to enter another math equation

