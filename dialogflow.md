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

All the others intents that you created are listed.

# Training Phrases

Once you have created the intent, you tell the bot what may trigger the intent. You tell the bot, what the user could say to refer to this intent. In other words, you train the bot. The bot will take this sentences to learn. That means, if the user tells something similar, the bot will be able to recognize it thanks to machine learning. For example:

- Tell me about your products.
- What are your products.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_648/v1525623705/Screen_Shot_2018-05-06_at_6.21.24_PM_qrhxfc.png)

## Responses

Here we explain to DialogFlow what we want to answer, if the customer triggers our intent.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525623946/Screen_Shot_2018-05-06_at_6.25.20_PM_kzgibr.png)

DialogFlow will pick one of our responses randomly.

# Entities

Say that the user can choose between 3 options for one particular thing. Say that he wants to order an icecrem, and you offer 3 categories: small, medium and big. These are entities for the type of icecream. In other words, the icecream can have the types small, medium or big. You can tell the bot some synonims for these words. Why? Because now, in your training phrases, the bot is going to recognize these entities.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525806785/Screen_Shot_2018-05-08_at_9.08.52_PM_urgft1.png)

Now in our training phrases, when we write a sentence, he will recognize the entities that we defined in the section Entities:

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_600/v1525808098/Screen_Shot_2018-05-08_at_9.34.33_PM_dcgdl1.png)

In our case, the bot recognizes the words large, big, small and assigns it to a parameter. Later on, we can work on this parameter.

In our response, we can use this information, since it was stored in our "variable".

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_600/v1525806785/Screen_Shot_2018-05-08_at_9.08.52_PM_urgft1.png)




# Integration of DialogFlow with other services

You can integrate your DialogFlow into other services. That makes answers funnier, since you can show cards, buttons etc.

- Facebook Messenger
- Web Page
- Slack
- Twitter
- etc.

As an example, we will use Facebook Messenger, since it's very easy to set up a Facebook Page.

# Integration with Facebook

We want to integrate our DialogFlow with our Facebook Messenger. In DialogFlow we define the conversation. Chances are that we have a Facebook page. By default, we have in Facebook the messenger chat. It would be nice to integrate our DialogFlow bot to our Facebook chat.

We go to the Facebook developeres app

```
https://developers.facebook.com/
```

The Developers Page gives us a lot of services to integrate to our page. We select the Facebook Messenger.

In the section, `my apps`, create a new app. Give it a name that describes your app. It should be related to your Facebook Page right?

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_300/v1525625806/Messenger_SetUp_fkfulw.png)

If we want to integrate a chatbot in our page, we need to create a Facebook app for this page:

Create app id

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525625870/newAppFB_jsohjz.png)

We need to generate a token for this app. A password. The token is used to give access to DialogFlow, when he tries to send information to our Facebook app. Imagine that you want to log in to Facebook. You need to have a password and enter it right? Between apps it's the same, but we use tokens, which are longer. So we need to create a token and give this token to DialogFlow, so that he can enter to our app.

![alt text](https://res.cloudinary.com/montolio/image/upload/v1525625665/FB_Token_png2uo.png)

We go back to our DialogFlow console and we paste this "Page Access Token"

We create a Verify Token. This is like a password, to access to DialogFlow. We will need to give this password to our Facebook app, so that the Facebook App can access our DialogFlow console.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_500/v1525625266/Screen_Shot_2018-05-06_at_6.47.07_PM_uu7kix.png)

# We create the webhook in the Facebook console.

![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_700/v1525625947/setupWebhook_agabu5.png)


In the Callback URL we put the URL that it was given to us in the DialogFlow console.

In verify token we enter the token that we created in the DialogFlow console.

We select messages and messaging_postbacks


![alt text](https://res.cloudinary.com/montolio/image/upload/c_scale,w_600/v1525625525/New_Page_Subscription_pvlmyk.png)

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






























