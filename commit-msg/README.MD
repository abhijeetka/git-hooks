 <h3> Git Commit-message hook for checking JIRA Ticket ID </h3>


<h5>Please find below the features that are provided by Commit Message hook.</h5>

It will check following things and allow to commit the code

1.	Branch name start from feature should have Jira ID.( E.g. : feature/Titck_ID-branch) . It will allow to commit a user only if the commit message contains the same JIRA ticket id present in Branch Name.

Ex : 
Branch Name: feature/PLAT-23-work
Valid Commit message: “PLAT-23 new work is going on”
Invalid Commit message: “PLAT-2 new work is goin on” OR “new work is goin on” OR “SSPORTAL-2 new work is goin on”

2.	Branch name start from release or develop or master will allow to commit if commit message contains the pattern that you have provided (E.g. : PLAT-any number, PE-any number).

Ex: 
Branch name : develop 
commit message: “No Pattern Added” -> Result= Fail
commit message: “ MUST Pass at least one of the patterns eg. PLAT-10  SSPORTAL-54 PLAT-5241” -> Result= PASS


3.	Branch name like lbs-bundle-php-unit-tests will allow to commit if commit message contains the pattern that you have provided (E.g. : PLAT-any number, PE-any number).

Ex:
Branch name: lbs-bundle-php-unit-tests
commit message: “No Pattern Added” -> Result= Fail
commit message: “ MUST Pass at least one of the patterns eg. PLAT-10  SSPORTAL-54 PLAT-5241” -> Result= PASS


if you want me to customize this hook, please let me know.
