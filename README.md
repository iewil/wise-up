# Why Wise-up?

This is an app to help you track your financial transactions from multiple credit/debit cards issued by multiple banks in Singapore.

Although there are already many financial tracking apps available for people to use, but the existing solutions each have their own limitations:

## Existing solutions

**Manual transaction tracking**)

*Examples: Spendee, Wally, Pocket Expense*

Pros:

This is easy to understand in terms of how the app works. These apps operate separately from all your banking services, and hence have the least exposure in terms of cyber security. 

Cons:

They are very tedious to use and oftern involve you having to manually save every transaction using the app in a structured format. Although some apps now include machine learning features to recognise text from receipts, they still have a low level of accuracy and still require the user to oftern intervene and correct mistakes in the results. 

Easy to use, but high required effort might deter even the most motivated people.

---

**Third-party expense tracking**

*Examples: Seedly*

Pros:

This is the most convenient way to track your expenses as the app will login to your account on your behalf, download and parse your transaction history and save consolidate your records from different banks into a single source. Users only have to provide the 2FA if it is a requirement of the bank. 

This services also provide tools to categorise expendentiture automatically.

Cons:

This encourages bad cybersecurity practices by having users provide their login credentials. Worst still, the credentials will have to to be stored on the servers in plain text. This is problematic because people tend to use the same set of login credentials accross mulitple servcices, and you have to trust that they only carry out the actions they've mentioned. 

---

## Objectives

1. Consolidate expenses from multiple sources
2. Do not pass credentials to third party providers

**NOTE!!** This project is a workaround while banks refuse to provide their users with API access. In the future, an OAuth-like authorisation protocol can be used to grant third party applications with prgrammatic access with limited scopes that has to be pre-approved by the user.

## Proposed approach

- Self-hosted transaction tracking.
- Get the open source community to contribute extensions for each bank

## Pre-requisite
- Node installed on your machine

**NOTE!!!** If you fork this repo for your own use, do not commit your login credentials into your git history.

## Getting started
- Download the repo
- 

## List of supported banks:

- UOB



==> pre-login
https://pib.uob.com.sg/PIBLogin/Public/processPreCapture.do?keyId=lpc&lang=en_SG

==> if there is an existing session
https://pib.uob.com.sg/PIBLogin/Public/processSubmit.do?token=292f21242081dfdc46bb047bf976bb32&keyId=0&_p=0&__c=15-3-C222F4EF0A7C6ABB01C27AE437FA2340

==> sucessful login (1FA)
https://pib.uob.com.sg/PIBCust/1FA/PIB.do?token=1c9150ebaadf6d3c289fce2858fac0c5

==> redirect to landing page
==> get list of accounts
==> trigger 2FA 
==> for each account, visit the account page
==> download the transaction history

