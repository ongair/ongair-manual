# Create a Contact

Sets up a contact in the contacts database. This acts as an opt-in before messages can be sent.

###Url

    https://app.ongair.im/api/v1/base/create_contact
    
###Method: 
POST

###Params:

|Field|		Type|	Mandatory	|Format|	Meaning
|----|----|---
|phone_number|		String|	Yes|	(country code)(phone number) e.g. 254722200200|	The contact phone number
|name|	String	|Yes|	Utf8 only encoded strings|	The contact name

###Response:
The server responds with a JSON message:

    {"created":true,"id":2067}
