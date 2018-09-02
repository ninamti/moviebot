# moviebot
A bot to get details of movies and actors

I am writing this bot using Dialog flow, a bot development framework by Google. 

Dialog flow allows users to create intents, entities and contexts to recognize 
speech / text. It also provides a way to fulfil those requests by calling backend 
services. I am using the OMDB (Open Movie Database) API to fulfil requests about 
movies.

The webhook for fulfilment is written in Javascript and uses node and express. 

Start the server by running `node index.js`

You should see a message saying `Server is up and running..`

This webhook needs to be deployed on a publicly available server. Google Cloud Function, 
Azure Function and AWS Lambda are examples of where this code can be deployed. 

To run it locally, 

One way to expose your code locally is to use `ngrok`. Use this guide to expose it locally. 

https://www.pluralsight.com/guides/exposing-your-local-node-js-app-to-the-world

`ngrok` gives you a URL that you need to enter in the fulfilment section of Dialogflow. 

  

