## say random stuff, then accept privacy policy - newsletter
* greet
    - utter_greet
    - utter_inform_privacypolicy
* greet OR enter_data OR contact_sales OR signup_newsletter OR human_handoff OR ask_builder OR ask_weather OR ask_howdoing OR ask_whatspossible OR out_of_scope OR thank OR ask_whoisit OR bye OR ask_whatisrasa
    - utter_must_accept
    - utter_inform_privacypolicy
* mood_confirm
    - utter_awesome
    - utter_ask_goal
* signup_newsletter
    - utter_great
    - utter_ask_email
* enter_data{"email": "maxmeier@firma.de"} OR enter_data{"number":"1"}
    - action_store_email
    - slot{"email": "maxmeier@firma.de"}
- action_subscribe_newsletter
    - slot{"subscribed": true}
    - utter_awesome
    - utter_confirmationemail
    - utter_docu
* mood_confirm
    - utter_thumbsup
    - utter_ask_feedback
* feedback{"feedback_value": "negative"}
    - slot{"feedback_value": "negative"}
    - utter_thumbsup
