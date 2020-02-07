## Response Node

### Usage

Response node is used to send a response to the user. We can send 2 types of responses:

1. Text Response
    a. To send a text response, you can simply write it in text form \
 \
![Image - Simple text response](https://content.convai.studio/docs/nodes/response/1.png)

    b. You can also extract variable data in the message script as well. For example, \
  \
![Image - Extract data image](https://content.convai.studio/docs/nodes/response/2.png)
 \
 \
You can use d, s or u depending on if the variable is saved in the execution, session or saved user data respectively.

    c. You can also add conditions based responses to the chatbot more. Refer to the [Go template documentation](/templating) for further tips and tricks \
 \
![Image - Conditions in response image](https://content.convai.studio/docs/nodes/response/3.png)

    d. To customize the response for a different channel, switch to the channel and add the response. If the channel response is not provided, the basic response will be sent on all the channels \
 \
![Image - Change response for channel](https://content.convai.studio/docs/nodes/response/4.png)
 

2. Text Message with Quick Replies (QR)
    a. To send a message with quick replies, just add {{ qr “qr name” “qr value” }}. Each QR has a name and value. Name is the text shown to the user but value is the text received back by the bot. If the value is not mentioned, the QR name is considered as the value by default. Examples, {{ qr “One” }} or {{ qr “One” “1” }}. Choose the format that works best for your case. \
 \
![Image - Send quick replies in responses](https://content.convai.studio/docs/nodes/response/5.png)


### Configuration

**Title** → Title of the node

**Send Now (Do not batch)** → Normally when a Convai request happens, all responses are collected and sent out at the end. When Send Now is enabled, the response will not wait until the request is finished. It will be sent immediately. Responses marked with Send Now will not be included when other batched messages are sent out at the end of a request.

**Channel** → Responses can be configured differently for different channels

**Message** → Message is a collection of messages. A single response can have more than 1 message. Click on ![Image - Addition Symbol](https://content.convai.studio/docs/nodes/response/6.png) to add more messages

**Message Editor** → The message editor is a [templating](/templating) enabled field where you can compose your response

**Typing Time** → Typing time defines the time to wait before sending the message to the user. During this time, the bot will show the typing indicator.
