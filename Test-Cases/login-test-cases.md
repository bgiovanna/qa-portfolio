# Login Test Cases

Application: Demo Website

| ID   | Test Case                    | Steps                               | Expected Result           |
| ---- | ---------------------------- | ----------------------------------- | ------------------------- |
| TC01 | Login with valid credentials | Enter valid username and password   | User logs in successfully |
| TC02 | Invalid password             | Enter valid user and wrong password | Error message displayed   |
| TC03 | Empty fields                 | Click login without entering data   | Validation error shown    |
| TC04 | Password case sensitivity    | Enter password with different case  | Login fails               |
| TC05 | Invalid username             | Enter non-existing user             | Error displayed           |
| TC06 | SQL injection attempt        | Enter `' OR 1=1` in username        | Login blocked             |
| TC07 | Long input                   | Enter very long username            | Validation message        |
| TC08 | Leading spaces               | Username with spaces                | Spaces trimmed            |
| TC09 | Session creation             | Successful login                    | Session token created     |
| TC10 | Logout after login           | Click logout                        | User session closed       |
