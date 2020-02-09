# Chatbot


Installation
- brew cask install miniconda
- conda install python=3.6
- conda create -n rasa python=3.6
- source activate rasa
- pip install rasa-x --extra-index-url https://pypi.rasa.com/simple
- //Go/Create the folder where you want your project to be
- rasa init

- Troubleshooting: https://towardsdatascience.com/create-chatbot-using-rasa-part-1-67f68e89ddad?gi=a5fd2f1beb58

Once everything installed, to run go to the Chatbot folder and:
- source activate rasa
- rasa x
- (In another terminal window) rasa run actions

How to train?
- Talk to your bot and start correcting the different mistakes. Once a full conversation has been done, save the Story.
- Once the story is saved, move to the Training tab, where you can correct the different doubts the system has.
- In the response tab, you can modify the responses or add new ones, always preceded by utter_X.
- Stories tab is important to edit how the flow of the conversation will be, try not having different stories with the same path and different responses, because that will make the system doubt.
- Lastly, touch the train button in the menu, and move to the Models tab, where you can select the new trained model, and delete the old ones. Only delete the old ones if you are sure that the new one works better.

REST API
- To talk to the bot through the REST API, which starts working whenever the RasaX has started running, just do a post request to localhost:5005/webhooks/rest/webhook where the body is:

  {
    "sender":"user",
    "message":"how old is marc"
  }

- There are also other calls to retrieve the whole conversation and other actions.

- To make it accessible from the internet, we can use: ngrok (brew cask install ngrok) running: ngrok http 5005 once the server is started. This command will redirect all the 5005-port traffic to a public IP address. Another option, no installs required is running ssh -R 80:localhost:5005 ssh.localhost.run
