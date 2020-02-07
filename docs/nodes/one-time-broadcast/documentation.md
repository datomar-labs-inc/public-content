## One Time Broadcast Node

### Usage

The one time broadcast is used to send an instant message to a user on any channel irrespective of the channel they are currently working on. It will only work if the channels are connected for the user.

For example, if the user is currently connected on Facebook Messenger and you want to send a verification code via SMS, add a one time broadcast node, select an SMS channel (like Twilio SMS) and then connect it to the flow you want to send.

Typically, a one time broadcast is followed by a response node.

![One Time Broadcast Node explained](https://content.convai.studio/docs/nodes/one-time-broadcast/1.png)

### Configuration

**Title** → The title of the node

**Asynchronous** → Determine if the message should be sent asynchronously or not

**Channel** → The channel on which the message should be sent

**Broadcast Type** → A custom name you can provide to the broadcast.