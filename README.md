#Saucedemo QA testing

A manual testing practice project on Saucedemo, a demo online shop built for testers. It has no real users or payments.

Tester: Akam Oluchi

#What I tested

- Login, including wrong password, empty fields and a locked-out user
- Sorting products by price
- Adding and removing items in the cart
- Product images and product detail pages

I tested with two accounts: `standard_user` (normal behaviour) and `problem_user` (built to contain bugs).

#How I tested

I wrote 12 test cases, ran each one by hand on Chrome on an Android phone, and recorded the result. When a test failed, I repeated it several times before reporting it, and recorded how often it failed.

#Results

- 12 test cases: 7 passed, 5 failed
- All failures were with `problem_user`
- 5 bugs logged in [Issues](https://github.com/oluchimiracle251-gif/Saucedemo-qa-testing/issues)

#Most interesting finding

Add to cart worked for only 3 of the 6 products on the products page (it failed in 3 of 4 attempts), but Remove worked correctly on the cart page. This suggests the problem is on the products page itself, and I noted that in the report.

#What I learned

- Repeat a failure before reporting it. One of my early "bugs" was a typing mistake.
- A good bug report has numbered steps, an expected result, an actual result, and how often it happens.
- A bug that happens in 3 of 4 attempts should be reported as exactly that, not as "always".

#Files

- [test-cases.md](test-cases.md)
- [Bug reports](https://github.com/oluchimiracle251-gif/Saucedemo-qa-testing/issues)

#Not done yet

- Exploratory testing session
- API testing
- Test automation
