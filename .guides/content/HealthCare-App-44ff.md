1) Uses https://fhir-dstu2.smarthealthit.org for patient information
2) Should be three pages - login, list of patients and when you click on the patient the app will display their patient details on the third page.
3) Hide the API key so nobody can find it
4) Use AsyncTask
5) Create unit tests
6) Mock out the web service

The URL for the api is https://fhir-api-dstu2.smarthealthit.org/

The API schema is defined at http://hl7.org/implement/standards/fhir/http.html

Sample API call
https://fhir-dstu2.smarthealthit.org/apps/fhir-demo/app/#/after-auth?code=Qwx66v&state=563ef72e-fc97-4af2-aeec-48c90828b83d

<h2>User Stories</h2>
**A user can login to their account**
As a user
I want to be able to login to an account
So that I can view patient information

**Acceptance Criteria**
**User enters correct credentials**
Given I am on the login screen
When i enter my username and password
And press the login button
Then I have logged in to my account
And I am taken to a screen showing a list of patients

**User enters incorrect credentials**
Given I am on the login screen
When I enter incorrect credentials
And press the login button
Then I receive an error message
<h2></h2>
**A User can view a list of patients**
As a user
I want to be able to view a list of patients
So that I can select a patient to view their patient details

**Acceptance Criteria**
**A list of patients is displayed with the patient's First and Last name**
Given I have entered correct login credentials
When I press 'login' on the login screen
Then I am taken to a screen showing a list of patients

<h2></h2>
**A user can view the patient details for a patient**
As a user
I want to see the details for a patient
So that I can view their patient data

**Acceptance Criteria**
**Selecting a patient from the patient list opens the patient details screen**
Given i am viewing a list of patients
When I select a patient from the list
Then i am taken to the patient details page for that patient

**Patient details screen shows the First name, Last name, date of birth, gender and address for the patient**
When I am on the patient details screen 
Then I can see the first and last name, date of birth, gender and address for the patient




