**Project Title**
Bitcoin Converter

**Project Description**

A convertor tool that converts Bitcoin to other currencies and vice versa.

In order to get the most recent Bitcoin to USD value an API is used

**How to test the Application**

This project has covered three tasks 

Task 1: Create a service class that will retrieve the value of Bitcoin vs a Currency and vice versa. Provide unit
tests

Service class is called 'BitcoinService'.cls
Apex Test Classes: 
- BitcoinServiceTest
- BitcoinServiceMock

This class makes a GET call to the Api to get currency rates which are later used in the page to display currencies. To quickly verify the result, use the below code snipped in execute anonymous and check the debug statement in the logs

BitcoinService.getValueOfBitcoinBasedOnCurrency('EUR');


Task 2: Build a page where a user can use Bitcoin convertor class to compare an amount in Bitcoin to different currencies.

The page has  the following requirements:

>> The user can enter a Bitcoin value or another currency
>> When a user changes the Bitcoin value, the other currency value would change automatically.
>> When the user would change the comparison currency value, the Bitcoin value would change
automatically.
>> Make sure the code is covered by unit tests.

The Visualforce page is called 'BitcoinConvertor'.page

Controller:
- BitcoinConvertorController

Apex Test Class: 
- BitcoinConvertorControllerTest

To see this page in action, switch to LEX and navigate to https://c.ap4.visual.force.com/apex/BitcoinConvertor

Enter an input for Bitcoin value and choose a currency, the value will be retrieved based on this combination automatically in the output field. Update the value in output field, the bitcoin value will be changed automatically as per currency conversion rates


Task 3: A manager wants to view a report on the most frequency requested comparisons. Build a report to
show the comparisons made, by user, and the most frequency currency requests that user has made.

Navigate to reports and open the report 'FrequentConversions' to view the latest comparisions

**Environment & Tools**
Salesforce
Force.com Migration Tool (ANT)

**Author**

Anudeep Gopagoni - anudeep.gopagoni@gmail.com
