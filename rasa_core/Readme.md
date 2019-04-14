# Process and command for running our chatbot on Facebook Messenger using Script Run
* From Rasa quickstart https://rasa.com/docs/core/quickstart/.
    1. Training our model(i.e it will create model folder in your directory)
         
      python -m rasa_core.train -d domain.yml -s stories.md -o models/dialogue
    
    2. Adding Natural Language Understanding(Nlu to our bot)
         
      python -m rasa_nlu.train -c nlu-config.yml --data nlu-data.md -o models --fixed_model_name nlu --project current --verbose
    
    3. We can talk with our bot through command line just to check whether it is working or not.
        
      python -m rasa_core.run --auth_token rasabot -d models\dialogue -u models\current\nlu -o out.log --endpoints endpoints.yml --enable_api
    
     *Note: It is updated command compare to rasa docs.*
     
     ![image](https://user-images.githubusercontent.com/39983195/56089615-3867e280-5eb3-11e9-921c-97310131ccbd.png)

     
    4. To connect on Facebook
        
      python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --endpoints endpoints.yml  --enable_api --debug
     
     *Note: It is updated command compare to rasa docs.* 
     
     5. Now we have to run **ngrok** in new command line.
      
      ngrok http 5002
      
     ![image](https://user-images.githubusercontent.com/39983195/56089697-71548700-5eb4-11e9-9846-451dfd7b7643.png)
      
     6. Run **actions** file in new command line.
    
      python -m rasa_core_sdk.endpoint --actions actions
    
     ![image](https://user-images.githubusercontent.com/39983195/56089856-18d2b900-5eb7-11e9-9cba-344d445405bb.png)

