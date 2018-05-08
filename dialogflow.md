Set of instructions to create a conversation in DialogFlow:

# Create your account in DialogFlow console

```
https://dialogflow.com/
```

- Sign Up
- Go to the console

# Create Agent

That's going to be your project. Here you create an agent (a project), for example, MyWebPageBot.

# Create Intent

Say that you want to respond if the user asks about your products. You want to create an intent which embraces this area.

Create intent with the name: `infoProducts`

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525623525/Screen_Shot_2018-05-06_at_6.18.12_PM_d3xg9i.png)

All the others intents are listed.

# Training Phrases

Once you have created the intent, you tell the bot what may trigger the intent. You tell the bot, what the user could say to refer to this intent. For example:

- Tell me about your products.
- What are your products.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_648/v1525623705/Screen_Shot_2018-05-06_at_6.21.24_PM_qrhxfc.png)

## Responses

Here we explain to DialogFlow what we want to answer, if the customer triggers our intent.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525623946/Screen_Shot_2018-05-06_at_6.25.20_PM_kzgibr.png)

DialogFlow will pick one of our responses randomly.

# Entities

We create the entity

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525806785/Screen_Shot_2018-05-08_at_9.08.52_PM_urgft1.png)

Are like parameters



# Integration of DialogFlow with other services

- Facebook Messenger
- Web Page
- Slack
- Twitter
- etc.

# Integration with Facebook

We want to integrate our DialogFlow with our Facebook Messenger. In DialogFlow we define the conversation. Changes are that we have a Facebook page. By defaultl, we have in Facebook the messenger chat. It would be nice to integrate our DialogFlow bot to our Facebook chat.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_300/v1525625806/Messenger_SetUp_fkfulw.png)

If we want to integrate a chatbot in our page, we need to create a Facebook app for this page:

Create app id

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525625870/newAppFB_jsohjz.png)

We need to generate a token for this app. The token is used to give access to DialogFlow, when he tries to send information to our Facebook app.

![alt text](https://res.cloudinary.com/montolio/image/upload/v1525625665/FB_Token_png2uo.png)

We go back to our DialogFlow console and we paste this "Page Access Token"

We create a Verify Token. This is like a password, to access to DialogFlow. We will need to give this password to our Facebook app, so that the Facebook App can access our DialogFlow console.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525625266/Screen_Shot_2018-05-06_at_6.47.07_PM_uu7kix.png)

# We create the webhook in the Facebook console.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_700/v1525625947/setupWebhook_agabu5.png)


In the Callback URL we put the URL that it was given to us in the DialogFlow console.

In verify token we enter the token that we created in the DialogFlow console.

We select messages and messaging_postbacks


![alt text](https://cloudinary.com/console/media_library#/dialog/image/upload/New_Page_Subscription_pvlmyk)

Our webhook is activated.

Now we select our Facebook page.



![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_600/v1525626047/webhookComplete_ltplst.png)

That's it!


# Funnier interaction with customers


Now that we have connected our DialogFlow with Facebook Messenger we can give as a response funnier things, like: 

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_250/v1525626381/addResponsesFunnier_hhoe2m.png)

# Fulfillment

Not just give text responses

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_600/v1525626491/textResponse_opl2pt.png)

But connect to your backend

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_700/v1525626588/webHookDFURL_bbjxqm.png)






























