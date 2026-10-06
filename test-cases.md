 #Test cases: Saucedemo

-Site: https://www.saucedemo.com
-Tester: Akam Oluchi
-Date: 06/10/2026
-Environment: Chrome on Android, Tecno Pop 7 Pro

 #Results with standard_user

| ID | Scenario | Expected | Actual | Result |
|----|----------|----------|--------|--------|
| TC-001 | Log in with correct details | Products page opens | Products page opened | Pass |
| TC-002 | Log in with wrong password | Error message; stay on login page | "Epic sadface: Username and password do not match any user in this service"| Pass |
| TC-003 | Log in with empty fields | Message that username is required |"Epic sadface: Username is required" | Pass |
| TC-004 | Log in as locked_out_user | Message that the user is locked out | "Sorry, this user has been locked out." | Pass |
| TC-005 | Sort by price, low to high | Prices go from lowest to highest | $7.99-$49.99 | Pass |
| TC-006 | Add one item to the cart | Button changes to Remove; cart shows 1 | As expected | Pass |
| TC-007 | Remove the item | Button changes back; cart number disappears | As expected | Pass |

 #Results with problem_user

| ID | Scenario | Expected | Actual | Result | Bug |
|----|----------|----------|--------|--------|-----|
| TC-008 | Look at product images | Each product shows its own picture | Pictures do not match product names | Fail | 1 |
| TC-009 | Add all six items to the cart | All six buttons respond | Only 3 respond (3 of 4 attempts) | Fail | 2 |
| TC-010 | Remove items on the products page | Items are removed | Remove buttons do nothing (4 of 4) | Fail | 3 |
| TC-011 | Sort by price | Order changes | Order stays the same | Fail | 4 |
| TC-012 | Open each product's page | Opens the tapped product | Wrong product or "Item not found" every time | Fail | 5 |

#Summary

- Test cases run: 12
- Passed: 7
- Failed: 5
- Bugs logged: 5 (see Issues)
