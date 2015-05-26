# Send Message

Method sends a text message to a single recipient

###Url:

    https://app.ongair.im/api/v1/base/send
    
###Method:

POST

###Params:

|Field|		Type|	Mandatory|Format|	Meaning
|---|
|phone_number|	String|	Yes|	(country code)(phone number) e.g. 254722200200	|Phone number to send to
|text|	String|	Yes	|Utf8 only encoded strings|	The message to be sent
|thread|	Boolean	|No	|true/false	|Whether the response should be in a conversation thread with the original message


###Response:

The server responds with a JSON message:

    {"sent":true,"id":2067}
    
|Field|	Type|	Meaning
|---|
|sent|		Boolean|	True or False if the image
|id	|Integer|	An Identifier for the message. This is used when delivering receipts

At this stage, the message has been sent to the WhatsApp server for delivery.
###Error:

If there is an error or the phone number does not exist, the server returns an error message and __*response code of 422*__.

    {"error":"Contact with phone number 25470586564 does not exists"}
    
    





