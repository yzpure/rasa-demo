## sales form
* contact_sales
    - utter_moreinformation
    - action_sales_form
    - form{"name": "action_sales_form"}
    - form{"name": null}

## sales form (no email)
* contact_sales
    - utter_moreinformation
    - action_sales_form
    - form{"name": "action_sales_form"}
* enter_data
    - utter_ask_email
* enter_data{"email": "123"}
    - action_sales_form
    - form{"name": null}
