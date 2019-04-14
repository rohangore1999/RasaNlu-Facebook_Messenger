# Process and command for running our chatbot on Facebook Messenger
* From Rasa quickstart https://rasa.com/docs/core/quickstart/.
    1. Training our model(i.e it will create model folder in your directory)
      - python -m rasa_core.train -d domain.yml -s stories.md -o models/dialogue
    
    2. Adding Natural Language Understanding(Nlu to our bot)
      - python -m rasa_nlu.train -c nlu-config.yml --data nlu-data.md -o models --fixed_model_name nlu --project current --verbose
    
    3. We can talk with our bot through command line just to check whether it is working or not.
     - python -m rasa_core.run --auth_token rasabot -d models\dialogue -u models\current\nlu -o out.log --endpoints endpoints.yml --enable_api
    
    * Note: It is updated comment compare to rasa docs. *
     
    4. To connect on Facebook
     - python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --endpoints endpoints.yml  --enable_api --debug
     
     * Note: It is updated comment compare to rasa docs. * 
     
