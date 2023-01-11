# Sample of sending Webex adaptive cards in Python

## Overview
This program is a simple and versatile sample for sending adaptive cards using json files output from the tool.
In addition to sending messages and attachments, Webex can also send graphical cards using Microsoft's adaptive card specification.
It is possible to add buttons, create choices, and of course, create items to be entered in free text.
For more information, please refer to the following guide
https://developer.webex.com/docs/buttons-and-cards

The content of the cards can be freely configured using the Buttons and Cards Designer.
https://developer.webex.com/buttons-and-cards-designer

When sending messages using Adaptive card in Python, use the json output from this tool.

To output json from this tool, click the button below. Save the json on the clipboard to a file.
[designer.png].
[json.png].

Store the python file and the output json file in the same hierarchy.
After that, adaptive cards can be sent to any user simply by running Python.

## important point
Run it on the Python 3 series.

request module is required.
Please install in advance.
> import requests

Enter the name of the file in which you saved the json output from Buttons and Cards Designer.
Or save the file as "card.json".
> fileName = "card.json"

Please enter the bot's access token.
> botToken = "<INSERT_AUTH_TOKEN_HERE>"

Please enter the e-mail address to which you would like to send the form.
> res = sendCard("<INSERT_DESTINATION_ADDRESS_HERE>", attachment)

To receive a reply to your card, use a webhook.
https://developer.webex.com/docs/api/guides/webhooks

Customize this to your liking.
