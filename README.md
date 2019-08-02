# User-MFA-Disabled-Status
This small script will get users in your AAD tenant who have not been enabled for MFA.

You'll need to call connect-msolservice before running this script. 
Note* There is not a state "Disbaled" for MFA. This script adds "Disabled" in the out put if the StrongAuthenticationRequirements.State attribute is null. Becasue the state is null it is safe to assume that MFA has not been enabled for the user. 

