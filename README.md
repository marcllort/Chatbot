# Chatbot

Follow tutorial: https://towardsdatascience.com/create-chatbot-using-rasa-part-1-67f68e89ddad?gi=a5fd2f1beb58

Once everything installed, to run go to the Chatbot folder and:
- source activate rasa
- rasa x
- (In another terminal window) rasa run actions

How to train?
- Talk to your bot, and start correcting the different mistakes. Once a full conversation has been done, save the Story.
- Once the story is saved, move to the Training tab, where you can correct the different doubts the system has.
- In the response tab, you can modify the responses or add new ones, always preceded byt utter_X.
- Stories tab is important to edit how the flow of the conversation will be, try not having different stories with the same path and  different responses, because that will make the system doubt.
- Lastly, touch the train button in the menu, and move to the Models tab, where you can select the new trained model, and delete the old ones. Only delete the old ones if you are sure that the new one works better.

