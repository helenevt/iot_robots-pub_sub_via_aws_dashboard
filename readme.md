### Make: IoT Robots
# PubSub via AWS Dashboard

![AWS IoT logo](/images/aws-iot-logo.jpg)

## Outcome

In performing this activity, you'll __subscribe and publish to a topic__ on the AWS IoT Dashboard, with a __formatted JSON message__. This message will be delivered to a message queue, and then appear in your Slack team channel.

## Introduction

A **message broker** is a pub/sub service used to send and receive messages between devices and apps. 

Each message is **published** to a **topic**, and the message broker then delivers those messages to all of the topic's **subscribers**. An useful analogy is a Slack channel: Each Slack channel is like a topic, and members can send (publish) messages to other members of the channel (subscribers).

![PubSub flow](/images/pubsub-flow.gif)

The messaging protocol we will be using is MQTT, specifically version 3.1.1. In more detailed activities, you will use websockets to send and receive MQTT messages, but for now you'll will use the AWS dashboard to communicate with the `makersPrep` topic we've set up.


## Activity

### Step 1: Sign into AWS IoT cloud with your maker account.

**Sign in page:** [https://offerzen-make.signin.aws.amazon.com/console](https://offerzen-make.signin.aws.amazon.com/console)  
**Credentials:** These have been mailed to you.


### Step 2: Navigate to IoT Cloud dashboard.

  ![IoT Cloud dashboard landing](images/aws_iot_landing.png)


### Step 3: In the sidebar menu, select **Test**.

  <img src="images/aws_iot_sidebar.png" width=200 />


### Step 4: Subscribe to the `makersPrep` topic.  

  <img src="images/aws_iot_subscribe.png" width=650 />


### Step 5: Publish a message to the `makersPrep` topic.

  **Message format:** a JSON object with attributes `"name"` as your full name, `"completed_prep"` as `true`, and an optional `"message"` string containing text of your choice.  

  <img src="images/aws_iot_publish.png" alt="images/aws_iot_publish.png" width=650 />


### Step 6: Check Slack!

If your message is successfully published and formatted correctly with the required data, **Maker Bot** on Slack will post to your team channel! 🤖🌈


### Stuck?

_If you need help, contact [@Nicholas Erasmus](https://offerzen-make.slack.com/messages/DA5HF1659) or [@Dan](https://offerzen-make.slack.com/messages/D9M8BBRNW) on Slack._



## Extra resources
- [AWS IoT Message Broker documentation](https://docs.aws.amazon.com/iot/latest/developerguide/iot-message-broker.html)


