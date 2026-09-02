# Application Exploration Notes

## 1. Login

### Observations

* Username field
* Password field
* Login button
* Forgot login information option
* Register option

### Questions to investigate

* What happens with valid credentials?
* What happens with invalid credentials?
* What happens when username is empty?
* What happens when password is empty?
* What happens when both fields are empty?
* What happens when a locked/non-existent account is used?

---

## 2. Registration

### Observations

## Fields
    * Name 
    * Last Name 
    * Address 
    * City
    * State
    * Zip code 
    * Phone number
    * SSN
    * Username
    * Password 
    * password confirmation

* Registration button



### Questions to investigate

* What fields are required?
* which fields are required and which are an option?
* What happens when required fields are empty?
* What happens when passwords do not match?
* Does the password have specific restrictions?
* Can an account be registered with an existing username?
* What happens after successful registration?

---

### 3. Account Servicess

## 3.1 Open New Account

### Observations 

## Fields 
* type of account 
* amount to be transfered to new account 
* open new account button

###Questions to Investigate

* What account types are available?
* Is selecting an account type mandatory?
* Is the transfer amount mandatory?
* What happens when the transfer amount is zero?
* What happens when the transfer amount is negative?
* What happens when the transfer amount exceeds the available balance?
* What happens when no source account is available?
* Is a new account number generated after successful account creation?
* Does the new account appear in Accounts Overview?

---

## 3.2 Account Overview

### Observations

** upon clicking "Account Overview" these area are displayed:

* Account number
* balance 
* Available amount 
* total

### Questions to Investigate

* Is the displayed balance accurate?
* Is the available amount accurate?
* What happens when multiple accounts exist?
* Does a newly opened account appear here?
* Does the balance update after a transfer?
* Does the balance update after a bill payment?
* Are transactions reflected correctly in the account information?
---

## 3.3 Transfers Funds

### Observations

* Amount (to be entered)
* From Account?
* To account?
* Transfer button

### Questions to investigate

* Can funds be transferred successfully?
* What happens with an invalid amount?
* What happens when the amount exceeds the available balance?
* Are source and destination accounts validated?
* Is the transaction reflected in the account balance?
* Does the transaction appear in transaction history?
* Can funds be transferred to the same account?
* Is the transaction reflected in the account balance?
* Does the transaction appear in transaction history?
* Is a confirmation message displayed after a successful transfer?

---

## 3.4 Bill Payment

### Observations

## Fields 
* Payee name
* Address
* City 
* State 
* zip code 
* Phone number 
* Account number 
* Verify account Number 
* Amount 
* From account 
* Send payment button 

### Questions to Investigate

* Which fields are mandatory?
* What happens when required fields are empty?
* What happens when the account numbers do not match?
* What happens when the payment amount is invalid?
* What happens when the payment amount exceeds the available balance?
* Is the payment processed successfully?
* Is the account balance updated?
* Does the payment appear in transaction history?
* Is a confirmation message displayed?

---

## 3.5 Find Transactions (Transaction History)

### Observations

## Fields
* Find by Transaction
* Select an account 
* Find by date 
* Find by date range
* Find by amount 

** all fields have " find transactions button "

### Questions to Investigate

* Can an existing transaction be found?
* What happens when no transaction matches the search criteria?
* What happens when an invalid date is entered?
* What happens when an invalid date range is entered?
* What happens when an invalid amount is entered?
* What happens when search fields are left empty?
* Are the returned transaction details accurate?

---

## 3.6 Update Contact Info

### Observations

## Fields
* same fields entered at registration, to be updated
** Update profile button

### Questions to Investigate

* Which fields can be updated?
* Which fields are mandatory?
* Can invalid information be submitted?
* Is the updated information saved successfully?
* Is a confirmation message displayed?
* Does the updated information persist after logging out and back in?

---

## 3.7 Request Loan 

### Observations

## Fields
* Loan Amount 
* Down Payment 
* From Acoount 
** Apply Now button

### Questions to Investigate

* What are the requirements for requesting a loan?
* What happens when the loan amount is invalid?
* What happens when the down payment is invalid?
* What happens when the down payment exceeds the loan amount?
* What happens when the selected account does not have sufficient funds?
* What happens after submitting a valid loan request?
* Is the loan request approved or rejected?
* Is a confirmation or status message displayed?

---

## 3.8 LogOut button

* A Log Out option is available to authenticated customers.

### Questions to Investigate

* Does selecting Log Out successfully end the session?
* Where is the customer redirected after logout?
* Can the customer access protected pages using the browser back button?
* Is the customer required to log in again after logout?

---

## 4. Navigation

### Observations ###

## 4.1 Solutions 
### Observation

* The Solutions option does not appear to be clickable or does not produce an observable navigation change during the initial exploration.


## 4.2 About Us 
### Observation

* The About Us option is available in the navigation.
* The page content changes when the option is selected

## 4.3 Services 
 * redirects different page

 ## 4.4 Products 
 * redirects 

## 4.5 Locations 
* redirects 

## 4.6 Admin Page 

### Observation
* Does not redirect but page info changes 

** Fields 
* Database: 
           * Initialise button 
           * Clean Button 
* JMS Service:
            * Status 
            * Shutdown button 
* Data Access Mode  
* Web Service:
           * Soap Endpoint (ParaBank Service)
           * Rest Endpoint (ParaBank Service)
           * Endpoint (LoanProcessor Service)
* Application Settings : 
           * Initial balnce 
           * Minimum balance 
           * Loan Provide 
           * Loan Processor 
           * Threshold
* Submit Button   

### Questions to Investigate

* Is the Admin Page intended for customers or administrators?
* Should it be included in customer-facing functional testing?
* What permissions are required to access it?
* Can an unauthorised customer access administrative functionality?
* What happens when administrative settings are changed?
* Are changes persisted after submission?

---

## 6. Potential Issues

* Solution is not clickable 
* Locations Link redirects to "Solutions" URL 

---

### 6. Initial Risk Observations

* Based on the functionality identified during exploration, the following areas appear to have higher testing priority:

# High Risk
* Authentication
* Registration
* Account creation
* Account balances
* Fund transfers
* Bill payments
* Transaction history
* Loan requests
# Medium Risk
* Forgot Login Information
* Update Contact Information
* Find Transactions
* Open New Account
# Lower Risk
* About Us
* Services
* Products
* Locations

