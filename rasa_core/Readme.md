# Process and command for running our chatbot on Facebook Messenger
* From Rasa quickstart https://rasa.com/docs/core/quickstart/.
  1. Training our model(i.e it will create model folder in your directory)
    - python -m rasa_core.train -d domain.yml -s stories.md -o models/dialogue
