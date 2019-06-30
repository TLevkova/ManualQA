[<sup>Return back to the project</sup>](/Animal-Project/README.md)

### TEST SUITE: REGISTRATION AND LOGIN

| Test Set               | Registration                                                                                         |
|:-----------------------|:-----------------------------------------------------------------------------------------------------|
| **TC59**               | **Register: All the required fields are marked with "\*"**                                           |
| Priority               | Medium                                                                                               |
| Description            | Verify that all the required fields are marked with asterisk "\*" and there is a legend indicating what the asterisk means - "Required fields"|
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Examine "Email" field | Asterisk symbol "\*" should be placed next to "Email" field title                                  |
| 2. Examine "Confirm Email" field | Asterisk symbol "\*" should be placed next to "Confirm Email" field title                  |
| 3. Examine "First Name" field | Asterisk symbol "\*" should be placed next to "First Name" field title                        |
| 4. Examine "Last Name" field | Asterisk symbol "\*" should be placed next to "Last Name" field title                          |
| 5. Examine "Date of Birth" field | Asterisk symbol "\*" should be placed next to "Date of Birth" field title                  |
| 6. Examine "Password" field | Asterisk symbol "\*" should be placed next to "Password" field title                            |
| 7. Examine "Confirm Password" field | Asterisk symbol "\*" should be placed next to "Confirm Password" field title            |
| 8. Check if there is a "Required Fields" notice under "Confirm Password" field | "Required Fields" notice is available and it's placed under "Confirm Password" field|
|                        |                                                                                                      |
| **TC60**               | **Register with valid credentials filling all the fields**                                           |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is able to register with valid credentials                                        |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
|Test Data               | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 5: +44 7700 900300<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted, no error message appears and "valid" icon appears next to the field|
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Click on "Contact Phone No." input box and enter phone number | The box is not highlighted and no error message appears    |
| 6. Click on "Male" radio button | "Male" radio button is selected                                                             |
| 7. Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears     |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Click on "Email" checkbox | The checkbox is selected                                                                      |
| 11. Click on "Post" checkbox | The checkbox is selected                                                                       |
| 12. Click on "Create Account" button | The user is registered and confirmation message is displayed                           |
| Postcondition          | Do not delete the user data from the database                                                        |
|                        |                                                                                                      |
| **TC61**               | **Register: Try to register with identical credentials**                                             |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register with credentials that already exist                         |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
|Test Data               | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 5: +44 7700 900300<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted, no error message appears and "valid" icon appears next to the field|
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Click on "Contact Phone No." input box and enter phone number | The box is not highlighted and no error message appears    |
| 6. Click on "Male" radio button | "Male" radio button is selected                                                             |
| 7.  Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears    |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Click on "Email" checkbox | The checkbox is selected                                                                      |
| 11. Click on "Post" checkbox | The checkbox is selected                                                                       |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
| Postcondition          | Delete the user data from the database                                                               |
|                        |                                                                                                      |
| **TC62**               | **Register with valid credentials filling the required fields only**                                 |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is able to register with valid credentials filling the required fields only (without optional fields)|
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
|Test Data               | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted, no error message appears and "valid" icon appears next to the field|
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Gender" button | No radio button is selected and no error message appers                              |
| 7.  Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears    |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is registered and confirmation message is displayed                           |
| Postcondition          | Delete the user data from the database                                                               |
|                        |                                                                                                      |
| **TC63**               | **Register: "Email" field - try to register with invalid email**                                     |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register with invalid email                                          |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
|Test Data               | Step 1: Use the email test data below<br>Step 2: Use the email test data below<br>Step 3: John<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| Email Test Data        | Email (Iteration 1): testing.animal.co.uk.gmail.com<br>Email (Iteration 2): testing.animal.co.uk@gmail<br>Email (Iteration 3): @gmail.com<br>Email (Iteration 4): testing.animal.co.uk@gmail..com<br>Email (Iteration 5): testing.animal.co.uk @gmail.com<br>Email (Iteration 6): kfdkjf<br>Email (Iteration 7): "; SELECT * FROM Users"|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter invalid email (Enter the information for the particular iteration) | The box is highlighted and error message appears|
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is highlighted and error message appears         |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Gender" button | No radio button is selected and no error message appers                              |
| 7.  Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears    |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
| Postcondition          | Repeat the test with the particular iteration's test data until you test all the possibilities       |
|                        |                                                                                                      |
| **TC64**               | **Register: "Email" field - try to register leaving "Email" field empty**                            |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register leaving empty "Email" field                                 |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
|Test Data               | Step 1: blank field<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Leave "Email" field blank | The box is highlighted and error message appears                                               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is highlighted and error message appears         |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty          | The box is not highlighted and no error message appears               |
| 6. Do not click on any "Gender" button | No radio button is selected and no error message appers                              |
| 7.  Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears    |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
|                        |                                                                                                      |
| **TC65**               | **Register: "Email" field - try to register leaving "Confirm Email" field empty**                    |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register leaving "Confirm Email" field empty                         |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: blank field<br>Step 3: John<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Leave "Confirm Email" field blank | The box is highlighted and error message appears                                       |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Gender" button | No radio button is selected and no error message appears                             |
| 7.  Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears    |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
|                        |                                                                                                      |
| **TC66**               | **Register: Try to register with mismatching emails**                                                |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register entering mismatching emails                                 |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and enter different еmail address | The box is highlighted and error message appears    |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Genfer" button | No radio button is selected and no error message apperas                             |
| 7.  Select day, month and year of birth in the drop-down menus | Selected items are displayed and no error message appears    |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
|                        |                                                                                                      |
| **TC67**               | **Register: "First Name" field - try to register with invalid data**                                 |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register with invalid first name                                     |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: Use the first name test data below<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123<br>|
| First Name Test Data   | First Name (iteration 1): 123456789<br>First Name (iteration 2): ~!@#$%^&\*()-=\_+[]{}\|;’”<>/?<br>First Name (iteration 3): (space)<br>First Name (iteration 4):  https://example.com<br>First Name (iteration 5): "; SELECT * FROM Users"|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted and no error message appears  |
| 3. Click on "First Name" input box and enter invalid first name (Enter the information for the particular iteration) | The box is highlighted and error message appears|
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Genfer" button | No radio button is selected and no error message apperas                             |
| 7.  Select day, month and year of birth in the dorop-down menus  | Selected items are displayed and no error message appears  |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
| Postcondition          | Repeat the test with the particular iteration's test data until you test all the possibilities       |
|                        |                                                                                                      |
| **TC68**               | **Register: "First Name" field - try to register leaving "First Name" field empty**                  |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register leaving "First Name" field empty                            |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: blank field<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted and no error message appears  |
| 3. Leave "First Name" field blank | The box is highlighted and error message appears                                          |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Genfer" button | No radio button is selected and no error message apperas                             |
| 7.  Select day, month and year of birth in the dorop-down menus | Selected items are displayed and no error message appears   |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
|                        |                                                                                                      |
| **TC69**               | **Register: "Last Name" field - try to register with invalid data**                                  |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register with invalid last name                                      |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Use the first name test data below<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| Last Name Test Data    | Last Name (iteration 1): 123456789<br>Last Name (iteration 2): ~!@#$%^&\*()-=\_+[]{}\|;’”<>/?<br>Last Name (iteration 3): (space)<br>Last Name (iteration 4):  https://example.com<br>Last Name (iteration 5): "; SELECT * FROM Users"|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted and no error message appears  |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter  invalid last name  (Enter the information for the particular iteration) | The box is highlighted and error message appears|
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Genfer" button | No radio button is selected and no error message apperas                             |
| 7.  Select day, month and year of birth in the dorop-down menus | Selected items are displayed and no error message appears   |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
| Postcondition          | Repeat the test with the particular iteration's test data until you test all the possibilities       |
|                        |                                                                                                      |
| **TC70**               | **Register: "Last Name" field - try to register leaving "Last Name" field empty**                    |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register leaving "Last Name" field empty                             |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: blank field<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted and no error message appears  |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Leave "First Name" field blank | The box is highlighted and error message appears                                          |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any "Genfer" button | No radio button is selected and no error message apperas                             |
| 7.  Select day, month and year of birth in the dorop-down menus | Selected items are displayed and no error message appears   |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
|                        |                                                                                                      |
| **TC71**               | **Register: "Contact Phone No." field - try to register with invalid data**                          |
| Priority               | Medium                                                                                               |
| Description            | Verify that a user is unable to register with invalid phone number                                   |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 5: Use the contact phone number test data below<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| Contact Phone No. Test Data | Contact Phone No. (iteration 1): abcdefghijk<br>Contact Phone No. (iteration 2): ~!@#$%^&\*()-=\_+[]{}\|;’”<>/?<br>Contact Phone No. (iteration 3): 1<br>Contact Phone No. (iteration 4): +44 7700 900300 1<br>Contact Phone No. (iteration 5): 44 7700 900300 1<br>Contact Phone No. (iteration 6): (space)<br>Contact Phone No. (iteration 7): https://example.com<br>Contact Phone No. (iteration 8): "; SELECT * FROM Users"|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted, no error message appears and "valid" icon appears next to the field|
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Click on "Contact Phone No." input box and enter invalid phone number | The box is highlighted and error message appears   |
| 6. Do not click on any "Genfer" button | No radio button is selected and no error message apperas                             |
| 7.  Select day, month and year of birth in the dorop-down menus | Selected items are displayed and no error message appears   |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
| Postcondition          | Repeat the test with the particular iteration's test data until you test all the possibilities       |
|                        |                                                                                                      |
| **TC72**               | **Register: "Gender" radio buttons - try to make multiple selection**                                |
| Priority               | Medium                                                                                               |
| Description            | Verify that a user is unable to make multiple selection clicking on "Gender" radio buttons           |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Action                 | Click on both "Gender" buttons and try to make multiple selection                                    |
| Expected result        | Only the last selection is made and multiple selection is not allowed                                |
|                        |                                                                                                      |
| **TC73**               | **Register: "Date of Birth" drop-down menus - try to register with invalid data**                    |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register with invalid date of birth                                  |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 7:  Use the date of birth test data below<br>Step 8: P@ssword123<br>Step 9: P@ssword123|
| Date of Birth Test Data| Date of Birth (iteration 1): Day-01-1991 (do not select anything in "Day" drop-down menu)<br>Date of Birth (iteration 2): 01-Month-1991 (do not select anything in "Month" drop-down menu)<br>Date of Birth (iteration 3): 01-01-Year (do not select anything in "Year" drop-down menu)<br>Date of Birth (iteration 4): 31-02-1991 (invalid day of month)<br>Date of Birth (iteration 5): 31-02-2009 (age prohibited by law)<br>Date of Birth (iteration 6): 10-06-2019 (invalid age)<br>Date of Birth (iteration 7): 31-12-2019 (date greater than the current date)|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box and enter еmail address | The box is not highlighted and no error message appears               |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted, no error message appears and "valid" icon appears next to the field|
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Click on "Contact Phone No." input box and enter phone number | The box is not highlighted and no error message appears    |
| 6. Do not click on any gender button | No radio button is selected and no error message apperas                               |
| 7.  Select invalid date of birth | The box is highlighted and error message appears                                           |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and repeat the password | The box is not highlighted and no error message appears    |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
| Postcondition | Repeat the test with the particular iteration's test data until you test all the possibilities                |
|                        |                                                                                                      |
| **TC74**               | **Register: "Password" field - try to register with invalid data**                                   |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register with invalid password                                       |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 7:  01-01-1991<br>Step 8: Use the password test data below<br>Step 9: Use the password test data below|
| Password Test Data     | "Password (iteration 1): ~!@#$%^&\*()-=\_+[]{}\|;’”<>/?<br>Password (iteration 2): Ab3<br>Password (iteration 3): Abcdef7<br>Password (iteration 4): (space)<br>Password (iteration 5):  https://example.com<br>Password (iteration 8): "; SELECT * FROM Users"|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box enter valid еmail address | The box is not highlighted and no error message appears             |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted and no error message appears  |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any gender button | No radio button is selected and no error message apperas                               |
| 7.  Select day, month and year of birth in the dorop-down menus | Selected items are displayed and no error message appears   |
| 8. Click on "Password" input box and enter invalid password | The box is highlighted and error message appears                |
| 9. Click on "Confirm Password" input box and repeat the password | The box is highlighted and error message appears           |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
|                        |                                                                                                      |
| **TC75**               | **Register: "Password" field - password is in encrypted format when entered**                        |
| Priority               | High                                                                                                 |
| Description            | Verify that the password is in encrypted format when is entered by the user                          |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Action                 | Click on "Password" input box and enter random text                                                  |
| Expected result        | The password is displayed in encrypted fromat                                                        |
|                        |                                                                                                      |
| **TC76**               | **Register: "Confirm Password" field - password is in encrypted format when entered**                |
| Priority               | High                                                                                                 |
| Description            | Verify that the password is in encrypted format when is entered by the user                          |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Action                 | Click on "Confirm Password" input box and enter random text                                          |
| Expected result        | The password is displayed in encrypted fromat                                                        |
|                        |                                                                                                      |
| **TC77**               | **Register: Try to register with mismatching passwords**                                             |
| Priority               | High                                                                                                 |
| Description            | Verify that a user is unable to register entering mismatching passwords                              |
| Precondition           | 1. Open [https://www.animal.co.uk](https://www.animal.co.uk)<br>2. Click on "Register" link at the top-right corner of the page|
| Test Data              | Step 1: testing.animal.co.uk@gmail.com<br>Step 2: testing.animal.co.uk@gmail.com<br>Step 3: John<br>Step 4: Doe<br>Step 7: 01-01-1991<br>Step 8: P@ssword123<br>Step 9: P@ssword1234|
| _**Test Steps**_       | _**Expected result**_                                                                                |
| 1. Click on "Email" input box enter valid еmail address | The box is not highlighted and no error message appears             |
| 2. Click on "Confirm Email" input box and repeat the еmail address | The box is not highlighted and no error message appears  |
| 3. Click on "First Name" input box and enter first name | The box is not highlighted and no error message appears             |
| 4. Click on "Last Name" input box and enter last name | The box is not highlighted and no error message appears               |
| 5. Leave "Contact Phone No." input box empty | The box is not highlighted and no error message appears                        |
| 6. Do not click on any gender button | No radio button is selected and no error message apperas                               |
| 7.  Select day, month and year of birth in the dorop-down menus | Selected items are displayed and no error message appears   |
| 8. Click on "Password" input box and enter password | The box is not highlighted and no error message appears                 |
| 9. Click on "Confirm Password" input box and enter different password | The box is highlighted and error message appears      |
| 10. Do not click on "Email" checkbox | The checkbox is not selected                                                           |
| 11. Do not click on "Post" checkbox | The checkbox is not selected                                                            |
| 12. Click on "Create Account" button | The user is not allowed to proceed and error message appears                           |
