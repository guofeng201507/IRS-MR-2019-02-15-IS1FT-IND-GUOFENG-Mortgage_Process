# ISS_MR_INDIVIDUAL_GF
Individual Assignment

This individual assignment is based on the sample project Mortgage_Process in KIE workbench. 

The changes added is to have an additional check for number of credit cards to determine the mortgage loan value, if the applicant has more than 10 credit card, mortgage should not be issued.

1. Introducing a new field "No of Credit Cards" in applicant data object.
2. Update forms with the new input field
3. Add new condition, combining with existing decision table logic.

Pre-requisite:
1. Make sure ID "jack" has group assigned as "iss-group-requestor"
2. Make sure ID "wbadmin" has group assigned as "iss-group-approver"


Steps to Verify:
1. Login as "jack", trigger instance and enter income as "110000", property price as "250000", property age as "4", location "Urban", number of credit card as "4", submit.
2. Login asa "wbadmin" and go to inbox, "mortage amount" should shown as "200000".

1. login as "jack", trigger instance and enter income as "110000", property price as "250000", property age as "4", location "Urban", number of credit card as "20", submit.
2. Login asa "wbadmin" and go to inbox, there will be no value for "mortgage".
