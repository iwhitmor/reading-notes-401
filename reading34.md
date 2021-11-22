# Payment Processing

## [How to read technical documentation](https://www.linkedin.com/pulse/20140730081025-316694350-how-to-read-technical-docs-in-the-minimum-time-possible/)

* 1. Establish why you are reading it

  * You want to establish why you are reading it so you can find what you need to find. If you don't know what you are trying to find you  might not pay much attention to it

* 2. Get an overview of the content and structure of the document

  * Make sure to read the cover, table of contents, and any intro chapter

* 3. Take 30 seconds - 2 minutes to skim rest of the doc

  * Look for things that are familiar to you (pictures etc)

* 4. If you want, stop at the interesting parts and take a deeper look. Stop when it gets boring

* 5. Look at the table of contents again. You'll have a deeper understanding of the document after you look again

* 6. Choose what to read next based on interesting-ness or usefulness. If there's nothing useful, close the doc. You can say that you've read it from cover to cover

## [How Credit Card Processing Works](https://wallethub.com/edu/cc/credit-card-transaction/25511)

* Credit card transaction process

  * Stage 1: Authorization

    * Merchant must obtain approval for payment from the issuing bank

  * Stage 2: Authentification

    * The issuing bank verifies the validity of the customer’s credit card using fraud protection tools such as the Address Verification Service (AVS) and card security codes such as CVV, CVV2, CVC2 and CID

  * Stage 3: Clearing and settlement

    * In the clearing stage, the transaction is posted to both the cardholder’s monthly credit card billing statement and the merchant’s statement. It occurs simultaneously with the settlement stage

* Credit card transaction participants

  * Cardholder

  * Merchant

  * Acquiring bank/merchant bank

  * Acquiring Processor/Service Provider

  * Credit Card Network/Association Member

  * Issuing Bank/Credit Card Issuer

* When a credit card transaction gets declined

  * When a credit card is declined, the point of sale (POS) terminal will return a response code that explains why. Sometimes those codes don’t tell the full story. In those instances, only your credit card issuer can identify the particular reason for the rejection, so you may need to call customer service to resolve the problem

## [How ONLINE Credit Card Processing Works](https://www.eventrebels.com/online-credit-card-processing-work/)

* Merchant Accounts

  * Merchant acct is how you connect to credit card processing network, which makes sure they are processed correctly and safely

* Payment gateway

  * The Payment Gateway is responsible for sending the credit card to the appropriate Internet Merchant Account over secure online channels

  * It is helpful to think of the Gateway as a router that sends the credit card information to the appropriate account.  It is also responsible for fraud checking and maintaining reliable links with the merchant

* Application

  * Summary of how the process would work if you had an application such as online registration:

    * User enters credit card information into the application
  
    * Credit card information is sent to the Payment Gateway via a secure channel
  
    * The Payment Gateway routes the credit card to the appropriate Internet Merchant Account
  
    * Internet Merchant Account connects to the Merchant Account for credit card processing
  
    * The result is passed back to the Gateway and then the application

* Validation, Refunds, and Settlement

  * If the customer’s credit card is declined you will usually see a general message such as “there was a problem processing your credit card.”  For security reasons, the online user will usually not see the specific reasons for the failure, such as a decline

### Additional Resources

* [Authorize .NET Developer Docs](https://developer.authorize.net/api/reference/index.html)

* [Authorize .NET SDK](https://github.com/AuthorizeNet/sdk-dotnet)

* Some infomation taken from the links provided above
