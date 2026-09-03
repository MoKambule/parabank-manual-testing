# ParaBank Test Scenarios

## Authentication

| ID    | Test Scenario                       | Priority |
| ----- | ----------------------------------- | -------- |
| TS001 | Verify successful customer login    | High     |
| TS002 | Verify login with invalid username  | High     |
| TS003 | Verify login with invalid password  | High     |
| TS004 | Verify login with empty username    | High     |
| TS005 | Verify login with empty password    | High     |
| TS006 | Verify login with both fields empty | High     |
| TS007 | Verify customer logout              | High     |

## Registration

| ID    | Test Scenario                                    | Priority |
| ----- | ------------------------------------------------ | -------- |
| TS008 | Verify successful customer registration          | High     |
| TS009 | Verify registration with missing required fields | High     |
| TS010 | Verify registration with mismatched passwords    | High     |
| TS011 | Verify registration using an existing username   | Medium   |

## Account Management

| ID    | Test Scenario                                  | Priority |
| ----- | ---------------------------------------------- | -------- |
| TS012 | Verify customer can view account information   | High     |
| TS013 | Verify customer can open a new account         | High     |
| TS014 | Verify customer can view account history       | High     |
| TS015 | Verify customer can update contact information | Medium   |

## Transfer Funds 

| ID    | Test Scenario                                            | Priority |
| ----- | -------------------------------------------------------- | -------- |
| TS016 | Verify successful fund transfer                          | Critical |
| TS017 | Verify transfer with invalid amount                      | High     |
| TS018 | Verify transfer exceeding available balance              | Critical |
| TS019 | Verify source account validation                         | High     |
| TS020 | Verify destination account validation                    | High     |
| TS021 | Verify completed transfer appears in transaction history | Critical |

## Bill Payment

| ID    | Test Scenario                                | Priority |
| ----- | -------------------------------------------- | -------- |
| TS022 | Verify successful bill payment               | Critical |
| TS023 | Verify bill payment with missing information | High     |
| TS024 | Verify bill payment with invalid information | High     |

## Navigation

| ID    | Test Scenario                | Priority |
| ----- | ---------------------------- | -------- |
| TS025 | Verify Home navigation       | Low      |
| TS026 | Verify About Us navigation   | Low      |
| TS027 | Verify Services navigation   | Low      |
| TS028 | Verify Products navigation   | Low      |
| TS029 | Verify Locations navigation  | Low      |
| TS030 | Verify Contact Us navigation | Low      |

## Loans

| ID    | Test Scenario                             | Priority |
| ----- | ----------------------------------------- | -------- |
| TS031 | Verify customer can submit a loan request | High     |
| TS032 | Verify loan request validation            | High     |

## Find Transactions 

| ID    | Test Scenario                                   | Priority |
|------ | ------------------------------------------------| -------- |
| TS033 | verify correct and available account selected   | High     |
| TS034 | Verify transaction by Id that is exists         | High     |
| TS035 | verify date                                     | High     |
| TS036 | verify find date by range                       | Low      |
| Ts037 | verify amount                                   | Low      |

## Open New Account 

| ID    | Test Scenario                                   | Priority |
|------ | ------------------------------------------------| -------- |
| TS038 | verify type of account                          | High     |
| TS039 | verify minimum amount is deposited              | High     |
| TS040 | verify existing account for deposit             | High     |

