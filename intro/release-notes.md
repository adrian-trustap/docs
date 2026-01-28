# Release notes

## Oct 2025
### Oct 30, 2025
 Trustap transactions now support an optional `image_url` parameter. You can use this parameter to display an image of the item on the Trustap payment screen, making it clear which item the buyer is paying for. See our [guide](../guides/image-url.md) for more information.

 We've released Trustap lite. A new, light-weight Trustap API integration. See our [guides](../guides/transactions/trustap-lite/listing-intro.md) for more information.

### Oct 20,2025
 You can now use the Trustap API  to capture postage fees as part of the buyer payment in the Trustap payment screen. See our [guide](../guides/transactions/online/online-postage-fee.md) for more details.  

### Oct 8, 2025
 We've updated the Trustap API transactions to simplify process for enabling bank transfer payments. See our [online](../guides/transactions/online/online-int-path.md#step-5-buyer-transfers-funds) and [face-to-face](../guides/transactions/face-to-face/face-to-face-int-path.md#step-5-buyer-transfers-funds) guides for more information. 


    
## Sept 2025
### Sept 18, 2025
 We've updated the Trustap API to support multiple charge configurations that you can apply dynamically in your transaction flow. [Read our guide](../guides/charge-config.md) for more information. 


## July 2025
### July 4, 2025
 The Trustap API now supports users in Hong Kong with payouts in Hong Kong dollar, `HKD`.



## May 2025
### May 19, 2025
 The Trustap API now supports Turkish users with payouts in Turkish lira, `TRY`.


## April 2025
### April 2, 2025
 The Trustap API now supports metadata. [Read our guide](../guides/transactions/metadata.md) for more information.



## March 2025
###  March 18, 2025
Previously, the Trustap API only supported submitting order issues during the complaint period. The Trustap API now supports submitting order issues when there is a problem in the delivery of the item.

The Trustap API has been updated to give more reliable Royal Mail tracking results.


## February 2025
### February 28, 2025
 Listing has been added to the list of deprecated endpoints. These endpoints are no longer supported. We do not recommend using these endpoints.



## January 2025
### January 28, 2025
 The Trustap API now includes a new endpoint that supports creating a Stripe account session and retrieving that account client secret. See our [guide](../../apis/openapi/personal/personal%2Egetaccountsession) for more information.


## December 2024
### December 9, 2024
 The Trustap API now supports the Swiss Franc, `CHF`.


### December 2, 2024
 
The Trustap API no longer returns an error for some users when accessing  [instant payouts](../../apis/openapi/buyers-and-sellers/users%2Esetinstantpayouts), resolving a previous issue.



## November 2024
### November 29, 2024
 The Trustap API now has an updated [Shippo shipping rates](../../apis/openapi/online-shipping/basic%2Egetshipposhippingrates) endpoint that now  returns rates in the same currency as the transaction.

 The Trustap API now has an updated [Shippo shipping rates](../../apis/openapi/online-shipping/basic%2Egetshipposhippingrates) endpoint response that includes the Shippo `shipment_id`.

### November 20, 2024
 The Trustap API now has an updated [Shippo shipping rates](../../apis/openapi/online-shipping/basic%2Egetshipposhippingrates) endpoint that includes `currency`.

 The Trustap API has been updated to fix an issue where some users received an error when setting their [payment type](../../apis/openapi/online-payment/basic%2Esetpaymentmethodfortransaction).

### November 15, 2024
 The Trustap API now includes [integrated shipping](../guides/transactions/online/online-shipping.md).



## October 2024
### October 22, 2024
 The Trustap API now includes a new endpoint that supports for face-to-face transactions.

### October 14, 2024
 The Trustap API has been updated to improve the performance of transaction retrieval endpoints.

 The Trustap API now uses more [descriptive verification error messages](../../apis/openapi/personal/getadditionalidentitydocumentverificationstatus).

### October 8, 2024
 The Trustap API now supports payouts in Indian Rupee `INR`.

### October 1, 2024
 The Trustap API now supports bank transfer as a payment method for online transactions.

## September 2024
### September 18, 2024

 The Trustap API now supports transaction payment with a user's balance.


## August 2024
### August 19, 2024
 The Trustap API now supports splitting the buyer protection fee between a buyer and a seller.


## July 2024
### July 19, 2024
 To support users' access to Stripe accounts, the Trustap API now includes a set of endpoints for interacting with Stripe. [See our reference guide](../../apis/openapi/personal) for more information.

### July 4, 2024
 The Trustap API has been updated. Bank transfer payments now include `sort_code`.


## June 2024
### June 20, 2024
 The Trustap API no longer includes the option for `allow_last_4` in personal user verification.

 The Trustap API now includes a new endpoint to retrieve supported registration countries for a client. See our [reference guide](../../apis/openapi/clients/client%2Egetsupportedregistrationcountries) for more information.


### June 6, 2024
 The Trustap API now supports payouts in Pakistan Rupee `PKR`.



## May 2024
### May 13, 2024
 The Trustap API now supports payouts in United Arab Emirates Dirham  `AED`.

 The Trustap API now supports payouts in Hungarian Forint `HUF`.




## March 2024
### March 14, 2024
 The Trustap API webhooks have been updated to include events associated with [payment reviews](../concepts/webhooks.md#event-codes). You can now receive webhook events when payment reviews are successful or have failed.

### March 4, 2024
 The Trustap API now supports [webhooks](../concepts/webhooks.md) when payment review is successful or has failed.



## January 2024
### January 23, 2024
 The Trustap API now includes better error messaging for KYC when SSN upload fails.

 The Trustap API has been updated to include a new endpoint that returns a [user's balance](../../apis/openapi/buyers-and-sellers/users%2Egetbalances) in their currency. 

### January 17, 2024
 The Trustap API has been updated to include a new field `code` as a zip when a [facility](../../apis/openapi/online-shipping/) is `postal_office`.


### January 12, 2024
 The Trustap API has been updated to include two new endpoints to support shipping. Read our guides on [pick_up_point](../../apis/openapi/online-shipping/) and [delivery_point](../../apis/openapi/online-shipping/) to learn more.


