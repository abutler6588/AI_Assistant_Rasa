# AI_Assistant_Rasa-

Restaurant bot that will help you find a restaurant based upon location and cuisine. 

=========================
NLU Training Data

Sample Format 
=========================
## itnent: < intent_name >
- <list of utterances>
- ....
=========================
## intent: affirm
- yes
- indeed 
- of course
....
  
## intent: deny
- no
- never
- I dont think so 
- dont like that 

Core Training Data 

## resturantSearch_tellingLocation_tellignCusisine
 - resturant_search
  - utter_ask_location
 - telling location
  - action_set_location
  - slot {"location": "Mumbai"}
  - utter_affirm_location
  - utter_ask_cuisine
 - telling_cuisine{"cusisine": "italian"}
  - slot {"cusisine" : "italian"}
  - action_show_resturants
 - affirm
  - utter_goodybe
