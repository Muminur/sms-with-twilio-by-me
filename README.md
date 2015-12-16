# sms-with-twilio-by-me

from twilio.rest import TwilioRestClient

# put your own credentials here 
ACCOUNT_SID = ""
AUTH_TOKEN = ""

client = TwilioRestClient(ACCOUNT_SID, AUTH_TOKEN)

client.messages.create(
        body="test sms alert for my pi", from_="+12566694950", to="+8801823358686"
)

