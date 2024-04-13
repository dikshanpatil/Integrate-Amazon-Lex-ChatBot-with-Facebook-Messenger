# Integrate-Amazon-Lex-ChatBot-with-Facebook-Messenger
This repository contains detail description of how to Integrate Amazon Lex ChatBot with Facebook Messenger. 
Welcome to a new project! In this guide, we’ll embark on the journey of integrating Amazon Lex ChatBot with Meta Messenger. We will create chatbot for Restaurant and our chatbot will interact with user and allowing user to specify the location and date to book a table in restaurant.

# Step 1: Create an Amazon Lex ChatBot
 * Sign in to the AWS Management Console and open the Amazon Lex console.
 * Click "Create" and define the bot's name, output voice, and session timeout.
 * Create intents, slots, and sample utterances to define how the bot will interact with users.
    Sample Intent can be "GreetIntent" where you specify chatbot how to greet.
 * Build and test the bot within the Lex console.
    Test GreetIntent:

   
# Step 2: Creating a Facebook Page for Your Bot
 Every chatbot needs a stage, and in this case, it’s a Facebook Page. We’ll create a dedicated page for your bot, set up messaging settings, and ensure everything is ready.

# Step 3: Configuring Meta Developer Account
 * To connect with Facebook Messenger, we need to dive into the Facebook Developer world. You can just go to https://developers.facebook.com/.
 * Create a new account if you don’t have one.

# Step 4: Creating a Meta Dev App
  * With your account, first we need to create a new App for our AWS Lex Bot.
    
# Step 5: Creating a Facebook Messenger Webhook
  But first, what’s a Webhook, Anyway?
   In Tech Speak…
     Webhooks are like digital messengers that apps use to chat with each other. When something noteworthy happens, like a new message or a fresh post, a webhook is triggered. It sends a signal to another app, saying, “Hey, something just went down — you might wanna know!”
   Picture This: The Pizza Tracker
     Let’s break it down with a real-world example. You order pizza online, and there’s this nifty pizza tracker. Ever notice how it magically updates when your pizza is prepping, baking, and finally en route? That’s webhooks at play! Each status change triggers a webhook to update your tracker in real-time.

 *  First we need to configure the Token generation (the 2nd configuration after webhook), that we need to create a permission to generate an Access Token to tell AWS Lex to establish connection to the FB Messenger.
 *  You should select the FB Page that we created for this project.
 *  You will have two values here - 1. Access Token, 2. App Secret from our account to share to AWS Lex Bot so the bot can establish a connection between AWS and FB.

# Step 6: Connecting Amazon Lex with Facebook Messenger
  * We will add a new channel in our AWS Lex bot.
  * Paste the tokens from FB Messenger app to connect to AWS Lex bot, also the Alias is super important as well, so write a name that is easy to remember and that is accordingly to the chat.
  * Enter again to the Channel Integration we already created to get the Callback URL and copy it.

# Step 7: Configure FB Messenger to receive Callback and Lex Integration
  * Return to the FB Messenger Dashboard where we got the tokens, but in this time we will configure the Webhook and paste the AWS Lex Callback URL with the Alias token, and verify it.
  * Add permission for messages and confirm it.

# Step 8: Test and Deploy Your ChatBot
  * Test your chatbot within Facebook Messenger by sending messages and verifying the responses.
  * Review the logs and metrics in the Lex console to identify any issues or areas for improvement.
  * Deploy the bot to make it available to Facebook users, following Facebook's review and approval process.

# Facing Difficulties ?
    [AWS Lex Developer Guide](https://docs.aws.amazon.com/lex/latest/dg/what-is.html)
    [Faceboook Messenger Platform Guide](https://developers.facebook.com/docs/messenger-platform)
    
 

