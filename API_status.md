# Status

Status
Method returns a health check of the system.

###Method
GET

    Url:https://app.ongair.im/api/v1/base/status?token=<enter_token_here>

###Response
It returns the following json:

    {"success":true,"phone_number":"254727550098","status_message":"Hey","online":false}


|Field|Type|Meaning|
|-----|-----|
|phone_number|String|Phone number on which the account is registered|
|status_message	|String	|The current whatsapp status message
|online|	boolean	|True or false as to whether the whatsapp account is currently online

