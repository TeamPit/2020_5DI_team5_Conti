# Test Case Specification

## EG Service

| Author | Date | Description |
| --- | --- | --- |
|  Lazri, Balestra, Conti, Zambelli| 13/05/2020 | Architecture Document |



# 1 Introduction

This document provides the test cases to be carried out for the Eg Service website. Each item to be tested is represented by an individual test case. Each case details the input and expected outputs.


# 2 Test Cases: Application

| Test ID | 2.1 |
| --- | --- |
| Title | Correct Login |
| Feature | Login to www.eg\_service.com |
| Objective | Confirm that proper user id an password yields access to the website as expected. |
| Test Actions | 1. Go to the Eg Service website2. Select View Account option3. Enter login information |
| Expected Results | System displays account balance with option to logoff. |

| Test ID | 2.2 |
| --- | --- |
| Title | Incorrect Password |
| Feature | Login to www.eg\_service.com |
| Objective | Confirm that valid user id with an invalid password denies access to the website without leaving the user stranded. |
| Test Actions | 1. Go to the Eg Service website2. Select View Account option3. Enter invalid login information |
| Expected Results | System displays error message with option to try again. |

| Test ID | 2.3 |
| --- | --- |
| Title | Incorrect User E-Mail |
| Feature | Login to www.eg\_service.com |
| Objective | Confirm that invalid user id denies access to the website without leaving the user stranded. |
| Test Actions | 1. Go to the Eg Service website2. Select View Account option3. Enter invalid login information |
| Expected Results | System displays error message with option to try again. |

| Test ID | 2.4 |
| --- | --- |
| Title | Select Option View Locations |
| Feature | Display merchant locations accepting Eg Service |
| Objective | Confirm that a list of locations is displayed after the user selects the option. |
| Test Actions | 1. Go to the Eg Service website2. Select View Locations option |
| Expected Results | System displays list of merchants with addresses. |

| Test ID | 2.5 |
| --- | --- |
| Title | Select Option View Transactions |
| --- | --- |
| Feature | Display recent Eg Service account transactions. |
| --- | --- |
| Objective | Confirm that recent transactions are displayed properly. |
| --- | --- |
| Test Actions | 1. Go to the Eg Service website2. Select View Account option3. Select View Transactions option |
| --- | --- |
| Expected Results | System displays recent transactions legibly with option to logoff. |
| --- | --- |
|
 |
 |

| Test ID | 2.6 |
| --- | --- |
| Title | Registration |
| Feature | Sign in a user to the web site |
| Objective | Confirm that a user could sign in correctly to the website |
| Test Actions | 1. Go to the Eg Service website2. Select Sing in button3. Insert an email and a password |
| Expected Results | System register the user to website server |

| Test ID | 2.7 |
| --- | --- |
| Title | Articles |
| Feature | View all articles of the site |
| Objective | Confirm that a user could view all articles |
| Test Actions | 1. Go to the Eg Service website2. Select Sing in button3. Go to Articles |
| Expected Results | System displays all the articles |


# 2 Test Cases: Proxy Server

| Test ID | 3.1 |
| --- | --- |
| Title | Correct Login |
| Feature | Login to [www.eg\_service.com](http://www.eg_service.com/) via proxy server |
| Objective | Confirm that proper user id an password yields access to the website as expected. |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter correct login information3. Press submit |
| Expected Results | Site displays numeric balance for account. |

| Test ID | 3.2 |
| --- | --- |
| Title | Incorrect Password |
| Feature | Login to [www.eg\_service.com](http://www.eg_service.com/) via proxy server |
| Objective | Confirm that invalid password denies access to the website and returns an error. |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter login information as defined in test data3. Press submit4. View page source. |
| Expected Results | Error tag is evident in page source. |

| Test ID | 3.3 |
| --- | --- |
| Title | Incorrect User E-Mail Login |
| Feature | Login to [www.eg\_service.com](http://www.eg_service.com/) via proxy server |
| Objective | Confirm that invalid user id denies access to the website and returns an error. |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter login information as defined in test data3. Press submit4. View page source. |
| Expected Results | Error tag is evident in page source. |

| Test ID | 3.4 |
| --- | --- |
| Title | View Transactions via Proxy Server |
| Feature | View transaction history on [www.eg\_service.com](http://www.eg_service.com/) via proxy server |
| Objective | Confirm that transaction history is accessed and retrieved from the website correctly. |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter login information as defined in test data3. Press submit4. View page source. |
| Expected Results | Recent transactions are displayed and numbers match those on www.eg\_service.com |
