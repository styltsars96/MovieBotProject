# MovieBotProject
A chatbot for facebook messenger. This particular repository has the Node-Red Flow for it.

It needs a DialogFlow agent and a facebook messenger app to connect to.

It also needs: the regular node-red setup plus:

->modify settings.js to have the following:

functionGlobalContext: {

	apiai:require('apiai'),
	
	request:require('request')
	
}

->install the following (npm install):

apiai

request

You need to add access tokens to the messageWebHookController Node.

One for Facebook messenger app, one for Dialogflow.

You also need an API key  https://www.themoviedb.org/ and add it to the "GET MOVIE API" http request node.
