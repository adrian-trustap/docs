# Emails

Trustap keeps users and systems informed by sending notifications at key transaction milestones or actions in a transaction's life. These notifications come in the following two forms.

- **Emails** that are sent to end users (buyers, sellers).
- **Webhooks** that are sent to your system for automation (see [Webhooks Guide](./webhooks.md)).

Emails are sent to your users at key points to do the following.
1. Inform users of changes to the transaction.
2. Get a response from them to progress the transaction to the next state.

* The content and request for action of each email is tailored to the recipient and status of the transaction.
* All email notifications come from the following email address `noreply@support.trustap.com`.

The following is a sample email a seller receives when they pass shipping details for a transaction. 


## Online transaction emails
The following tables show the events and corresponding emails that Trustap send to buyers and sellers for online transactions.

### Payment

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Payment confirmed | Inform Buyer that their payment was successful | View transaction in Trustap app |
| Seller | Payment confirmation | Inform Seller that payment was successful | Submit tracking details |
| Buyer | Order processing  | Inform Buyer that their payment was successful and that their order would be processed |  |
| Buyer | Order failed to process | Inform Buyer that their payment was successful but their order failed to be processed |  |
| Buyer | Partial refund | Inform Buyer that their payment has been partially refunded by the Seller | View transaction in Trustap app |
| Seller | Partial refund | Inform Seller that they have partially refunded the Seller | View transaction in Trustap app |


### Tracking

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Seller | Add tracking details reminder | Remind Seller to add tracking details to the transaction | Submit tracking details |
| Seller | Tracking details added | Confirm tracking details were added to the transaction | View transaction in Trustap app |
| Buyer | Tracking details added | Inform Buyer that tracking details were added to the transaction | View transaction in Trustap app |
| Seller | Deadline extended to add tracking details | Inform Seller that the buyer has extended the deadline to add tracking details to the transaction | Submit tracking details |

### Complain

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Delivery confirmed | Inform Buyer that delivery has been confirmed and complaint period has begun | View transaction / Complain |
| Seller | Delivery confirmed | Inform Seller that delivery has been confirmed and complaint period has begun | Register for full Trustap account in preparation for payout |


### Funds released

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Funds released | Inform Buyer that transaction is complete and funds have been released to Seller |  |
| Seller | Funds released | Inform Seller that transaction is complete and funds have been released |  |


## Face-to-face transaction emails
The following tables show the events and corresponding emails that Trustap send to buyers and sellers for face-to-face transactions.


### Payment

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Payment Confirmed | Inform Buyer that their payment was successful | View transaction in Trustap app |
| Seller | Offer received | Inform Seller that an offer was received | Accept Payment |
| Buyer | Order processing  | Inform Buyer that their payment was successful and that their order would be processed |  |
| Buyer | Order failed to process | Inform Buyer that their payment successful but their order failed to be processed |  |
| Buyer | Payment accepted | Inform Buyer that their payment was accepted by the Seller | View transaction in Trustap app |
| Buyer | Payment rejected | Inform Buyer that their payment was rejected by the Seller | View transaction in Trustap app |
| Buyer | Partial refund | Inform Buyer that their payment has been partially refunded by the Seller | View transaction in Trustap app |
| Seller | Partial refund | Inform Seller that they have partially refunded the Seller | View transaction in Trustap app |


### Cancel

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Transaction cancelled | Confirm that Buyer has cancelled transaction | View transaction in Trustap app |
| Seller | Transaction cancelled | Inform Seller that transaction has been cancelled | View transaction in Trustap app |
| Seller | Transaction cancelled | Confirm that Seller has cancelled transaction | View transaction in Trustap app |
| Buyer | Transaction cancelled | Inform Buyer that transaction has been cancelled | View transaction in Trustap app |
| Buyer | Refund processed | Inform Buyer that transaction has been refunded | View transaction in Trustap app |
| Seller | Refund issued | Confirm that Buyer has been issued a refund | View transaction in Trustap app |

### Payment reminder

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Seller | Remainder skipped | Inform Seller that Buyer has skipped remainder payment | View transaction in Trustap app |
| Buyer | Remainder payment lodged | Confirm remainder payment has been made | View transaction / Complain |
| Seller | Remainder payment lodged | Confirm remainder payment has been made by Buyer | View transaction / Complain |

### Complaint

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Handover confirmed | Confirm with Buyer that item handover has been completed and complaint period has begun | Complain in Transaction page |
| Seller | Handover confirmed | Confirm with Seller that item handover has been completed and complaint period has begun | Register for full Trustap account in preparation for payout |
| Buyer | Handover confirmed | Inform Buyer that Seller has confirmed item handover and complaint period has begun | Complain in Transaction page |
| Seller | Handover confirmed | Inform Seller that Buyer has confirmed item handover and complaint period has begun | Register for full Trustap account in preparation for payout |


### Funds released

| Recipient | Topic | Purpose | Available actions |
|---|---|---|---|
| Buyer | Funds released | Inform Buyer that transaction is complete and funds have been released to Seller |  |
| Seller | Funds released | Inform Seller that transaction is complete and funds have been released |  |


## Customization
By default, your company brand is not displayed in Trustap emails to your buyers and sellers. Trustap does offer options for co-branded emails. Emails containing branding from both your company and Trustap help build user confidence. 

The following is an example co-branded email.


Co-branding is available in two parts.
1. Your company logo  and  company name in the email heading.
2. Your company name in the email body.

You can choose to add either or both options to your emails.

To enable your co-branded email, contact your Trustap integration specialist with the following details.
* Your preferred branding option (company name in body, company logo and name in heading, or both).
* Your preferred company name as it should appear in the email.
* A link to your company logo. We support Favicons (.ico), JPG, and PNG (preferred). 

## Testing
* For testing webhooks, refer to the [webhook test](./webhooks.md#testing) guide.
* For testing email notification, we recommend the following.
    1. Use an active test email account during integration.
    2. Follow step 1 to step 5 in either [online](../guides/transactions/online/online-int-path.md) or [face-to-face](../guides/transactions/face-to-face/face-to-face-int-path.md) transaction flow guides to trigger an email. 
    3. Watch your inbox for email samples.