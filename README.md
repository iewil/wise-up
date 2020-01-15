# Why Wise-up?

This is an app to help you track your financial transactions from multiple credit/debit cards issued by multiple banks in Singapore.

Although there are already many financial tracking apps available for people to use, but the existing solutions each have their own limitations:

**Manual transaction tracking**
*Examples: Spendee, Wally, Pocket Expense*

Manual they are either too tedious to use (having to manually save every transaction) or encourages bad cybersecurity practices (having to provide your login credentials to be stored on the applications server in plain text).

This is problematic because people tend to use the same set of login credentials accross mulitple servcices, and you have to trust that your 



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

