## story 01
* greet
  - utter_greet

## story 02
* goodbye
  - utter_goodbye

## story 04
* inform
  - utter_ask_location

## story 05
* inform{"location": "italy"}
  - slot{"location": "italy"}
  - action_weather
  - slot{"location": "italy"}

## greeting
* greet
  - utter_greet

## name goals
* my_name_is
  - utter_its_nice_to_meet_you

## gains and happy
* gains
  - utter_gains
  - utter_gains_up
  - utter_did_that_help
* mood_affirm
  - utter_happy

## gains and sad
* gains
  - utter_gains
  - utter_gains_up
  - utter_did_that_help
* mood_deny
  - utter_goodbye

## lose and happy
* lose
  - utter_lose
  - utter_lose_up
  - utter_did_that_help
* mood_affirm
  - utter_happy

## lose and sad
* lose
  - utter_lose
  - utter_lose_up
  - utter_did_that_help
* mood_deny
  - utter_goodbye