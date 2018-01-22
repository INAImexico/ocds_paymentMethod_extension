# Payment Method
## Description:

The payment method is a data that can be useful to understand the means by which payments associated with a contract are received. In Mexico, from INAI we have this information in our system and its publication is mandatory according to our Freedom to Information Act.

## Proposal:

Add a new field named “paymentMethod” to the transaction object.
  
### Schema

  - Transaction {object}
    - paymentMethod (string) (codelist)

The code list will be open and must be defined by:
  - Cash
  - Check
  - Wire transfer
  - Corporate credit card
  - Letter of credit
  
## Defining texts:

**Code** | **Title** | **Description**
--|--|--
paymentMethod | Payment method | The payment method used to make the transaction. The values of the paymentMethod codelist must be used (https://github.com/INAImexico/ocds_paymentMethod_extension/blob/master/codelists/paymentMethod.csv).
cash | Cash | The payment associated with this contract was made through cash.
check | Check | The payment associated with this contract was made by check.
wireTransfer | Wire transfer | The payment associated with this contract was made through a bank transfer.
corporateCard | Corporate card | The payment associated with this contract was made through a corporate credit card. Usually used to purchasing items directly for goods and services in the course of operations.
letterOfCredit | Letter of credit | The payment associated with this contract was made through a letter of credit. Letters of credit are used to guarantee that a supplier will receive a specified amount of money within a specified time providing strict terms.

## Issues 

Report issues for this extension in the [standard repository](https://github.com/open-contracting/standard/issues/622) of the Open Contracting Partnership.
