## happy path
* greet
  - utter_greet
* mood_great
  - action_hello_world

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## New Story

* name
    - utter_name

## New Story

* name
    - utter_name
* affirm
    - utter_greet

## New Story

* greet
    - utter_greet
* askMe
    - utter_happy
* greet
    - utter_askme

## New Story

* greet
    - utter_greet
* askMe
    - utter_happy
* greet
    - utter_askme
* affirm
    - utter_dontknow
    - action_default_ask_rephrase

## New Story

* greet
    - utter_greet
* askMe
    - utter_happy
* askMe
    - utter_askme
* dontknow
    - utter_dontknow
    - action_default_ask_rephrase

## New Story

* greet
    - utter_greet
* askMe
    - utter_happy
* askMe
    - utter_askme
* dontknow
    - utter_dontknow
    - action_default_ask_rephrase
* goodbye
    - utter_goodbye

## New Story

* helloworld
    - action_hello_world
