## Input Node

### Usage

The input node is used to gather data from the user. It is usually used after a response (Question) node. The input node pauses further interaction with the chatbot.

In order to continue the conversation from the same place, add higher priority to the connecting link between the input and the next node. For example, in the picture below, the link between the “User Feedback” has been given higher priority than the Normal Response.

Also note, “No Feedback Response” has been given the highest priority to factor for cases where the user doesn’t want to provide feedback.

![Input Node Explained](https://content.convai.studio/docs/nodes/input/1.png)

### Configuration

**Title** → Title of the node
