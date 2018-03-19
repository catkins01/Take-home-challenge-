# Take-home-challenge-
Challenge 1


Hi Amy, please create an account on our Dashboard. Once you’ve completed the signup process and acknowledged our terms, we’ll provide a live client_id, secret, and public_key on the Dashboard. This should resolve your issue accessing your item.
The difference between a public_token and a access_token is: 
public_token: A short-lived token that can be exchanged for an access_token or used to initialize Link in update mode for an Item.
access_token: A rotatable token unique to a single Item; used to access data for that Item.
Amy I do hope this answered your questions. 


Challenge 2


Hi George, after looking closely at the example you referenced in your question I believe the example itself was entered incorrectly.

Try this instead I pulled it from the documentation you mentioned:
curl -X POST https://sandbox.plaid.com/institutions/search \
  -H 'content-type: application/json' \
  -d '{
    "query": "BB&T",
    "products": ["transactions"],
    "public_key": String
  }'
  After you use the revised example provided above you should be able to search by bank and product without issue.
  Have a great day. 
  
  
  Challenge 3
  
  
  
  You have completed Plaid Link. View your accounts below.
$100.00
Plaid Checking - 0000
$200.00
Plaid Saving - 1111
$1,000.00
Plaid CD - 2222
($410.00)
Plaid Credit Card - 3333
$890
Total Assets

PNC was the bank I used. 
