python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --enable_api --debug



Microsoft Windows [Version 10.0.17134.648]
(c) 2018 Microsoft Corporation. All rights reserved.

C:\Users\Rohan Gore\Documents\Chatbot\rasabot\Scripts>activate
(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasabot\Scripts>cd ..

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasabot>cd ..

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot>cd rasa_core

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.train -d domain.yml -s stories.md -o models/dialogue
Processed Story Blocks: 100%|¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦| 4/4 [00:00<00:00, 1336.83it/s, # trackers=1]
Processed Story Blocks: 100%|¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦| 4/4 [00:00<00:00, 572.99it/s, # trackers=4]
Processed Story Blocks: 100%|¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦| 4/4 [00:00<00:00, 250.67it/s, # trackers=12]
Processed Story Blocks: 100%|¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦¦| 4/4 [00:00<00:00, 215.74it/s, # trackers=12]
2019-04-08 20:31:10.673889: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
_________________________________________________________________
Layer (type)                 Output Shape              Param #
=================================================================
masking (Masking)            (None, 5, 18)             0
_________________________________________________________________
lstm (LSTM)                  (None, 32)                6528
_________________________________________________________________
dense (Dense)                (None, 12)                396
_________________________________________________________________
activation (Activation)      (None, 12)                0
=================================================================
Total params: 6,924
Trainable params: 6,924
Non-trainable params: 0
_________________________________________________________________
2019-04-08 20:31:11 INFO     rasa_core.policies.keras_policy  - Fitting model with 62 total samples and a validation split of 0.1
Epoch 1/100
62/62 [==============================] - 2s 25ms/step - loss: 2.4695 - acc: 0.1452
Epoch 2/100
62/62 [==============================] - 0s 290us/step - loss: 2.4277 - acc: 0.1613
Epoch 3/100
62/62 [==============================] - 0s 306us/step - loss: 2.3976 - acc: 0.3065
Epoch 4/100
62/62 [==============================] - 0s 291us/step - loss: 2.3670 - acc: 0.3226
Epoch 5/100
62/62 [==============================] - 0s 289us/step - loss: 2.3530 - acc: 0.3387
Epoch 6/100
62/62 [==============================] - 0s 306us/step - loss: 2.3142 - acc: 0.4355
Epoch 7/100
62/62 [==============================] - 0s 290us/step - loss: 2.2819 - acc: 0.4677
Epoch 8/100
62/62 [==============================] - 0s 322us/step - loss: 2.2582 - acc: 0.4032
Epoch 9/100
62/62 [==============================] - 0s 274us/step - loss: 2.2162 - acc: 0.4355
Epoch 10/100
62/62 [==============================] - 0s 290us/step - loss: 2.1915 - acc: 0.4355
Epoch 11/100
62/62 [==============================] - 0s 290us/step - loss: 2.1664 - acc: 0.4355
Epoch 12/100
62/62 [==============================] - 0s 338us/step - loss: 2.1500 - acc: 0.4355
Epoch 13/100
62/62 [==============================] - 0s 273us/step - loss: 2.0952 - acc: 0.4194
Epoch 14/100
62/62 [==============================] - 0s 291us/step - loss: 2.0667 - acc: 0.4355
Epoch 15/100
62/62 [==============================] - 0s 307us/step - loss: 2.0798 - acc: 0.4355
Epoch 16/100
62/62 [==============================] - 0s 301us/step - loss: 2.0015 - acc: 0.4355
Epoch 17/100
62/62 [==============================] - 0s 304us/step - loss: 1.9772 - acc: 0.4355
Epoch 18/100
62/62 [==============================] - 0s 289us/step - loss: 1.9268 - acc: 0.4355
Epoch 19/100
62/62 [==============================] - 0s 306us/step - loss: 1.8797 - acc: 0.4355
Epoch 20/100
62/62 [==============================] - 0s 273us/step - loss: 1.8775 - acc: 0.4355
Epoch 21/100
62/62 [==============================] - 0s 290us/step - loss: 1.8367 - acc: 0.4355
Epoch 22/100
62/62 [==============================] - 0s 274us/step - loss: 1.7907 - acc: 0.4355
Epoch 23/100
62/62 [==============================] - 0s 354us/step - loss: 1.7468 - acc: 0.4355
Epoch 24/100
62/62 [==============================] - 0s 292us/step - loss: 1.7781 - acc: 0.4355
Epoch 25/100
62/62 [==============================] - 0s 306us/step - loss: 1.7276 - acc: 0.4355
Epoch 26/100
62/62 [==============================] - 0s 274us/step - loss: 1.7334 - acc: 0.4355
Epoch 27/100
62/62 [==============================] - 0s 297us/step - loss: 1.7125 - acc: 0.4355
Epoch 28/100
62/62 [==============================] - 0s 289us/step - loss: 1.6811 - acc: 0.4355
Epoch 29/100
62/62 [==============================] - 0s 277us/step - loss: 1.6770 - acc: 0.4355
Epoch 30/100
62/62 [==============================] - 0s 322us/step - loss: 1.6796 - acc: 0.4355
Epoch 31/100
62/62 [==============================] - 0s 290us/step - loss: 1.6385 - acc: 0.4355
Epoch 32/100
62/62 [==============================] - 0s 338us/step - loss: 1.6222 - acc: 0.4355
Epoch 33/100
62/62 [==============================] - 0s 306us/step - loss: 1.6300 - acc: 0.4355
Epoch 34/100
62/62 [==============================] - 0s 290us/step - loss: 1.6199 - acc: 0.4355
Epoch 35/100
62/62 [==============================] - 0s 297us/step - loss: 1.5993 - acc: 0.4355
Epoch 36/100
62/62 [==============================] - 0s 309us/step - loss: 1.5826 - acc: 0.4355
Epoch 37/100
62/62 [==============================] - 0s 322us/step - loss: 1.5857 - acc: 0.4355
Epoch 38/100
62/62 [==============================] - 0s 306us/step - loss: 1.5627 - acc: 0.4355
Epoch 39/100
62/62 [==============================] - 0s 290us/step - loss: 1.5583 - acc: 0.4355
Epoch 40/100
62/62 [==============================] - 0s 306us/step - loss: 1.5828 - acc: 0.4355
Epoch 41/100
62/62 [==============================] - 0s 290us/step - loss: 1.5500 - acc: 0.4355
Epoch 42/100
62/62 [==============================] - 0s 306us/step - loss: 1.5488 - acc: 0.4355
Epoch 43/100
62/62 [==============================] - 0s 278us/step - loss: 1.5117 - acc: 0.4355
Epoch 44/100
62/62 [==============================] - 0s 305us/step - loss: 1.5069 - acc: 0.4355
Epoch 45/100
62/62 [==============================] - 0s 306us/step - loss: 1.5230 - acc: 0.4355
Epoch 46/100
62/62 [==============================] - 0s 305us/step - loss: 1.4871 - acc: 0.4355
Epoch 47/100
62/62 [==============================] - 0s 292us/step - loss: 1.4882 - acc: 0.4355
Epoch 48/100
62/62 [==============================] - 0s 290us/step - loss: 1.4721 - acc: 0.4355
Epoch 49/100
62/62 [==============================] - 0s 306us/step - loss: 1.4862 - acc: 0.4355
Epoch 50/100
62/62 [==============================] - 0s 311us/step - loss: 1.4750 - acc: 0.4516
Epoch 51/100
62/62 [==============================] - 0s 290us/step - loss: 1.4513 - acc: 0.4355
Epoch 52/100
62/62 [==============================] - 0s 290us/step - loss: 1.4250 - acc: 0.4516
Epoch 53/100
62/62 [==============================] - 0s 290us/step - loss: 1.4499 - acc: 0.4355
Epoch 54/100
62/62 [==============================] - 0s 287us/step - loss: 1.4492 - acc: 0.4516
Epoch 55/100
62/62 [==============================] - 0s 306us/step - loss: 1.4121 - acc: 0.4677
Epoch 56/100
62/62 [==============================] - 0s 290us/step - loss: 1.4216 - acc: 0.4677
Epoch 57/100
62/62 [==============================] - 0s 306us/step - loss: 1.3998 - acc: 0.4516
Epoch 58/100
62/62 [==============================] - 0s 290us/step - loss: 1.3922 - acc: 0.4516
Epoch 59/100
62/62 [==============================] - 0s 290us/step - loss: 1.3874 - acc: 0.4677
Epoch 60/100
62/62 [==============================] - 0s 295us/step - loss: 1.3862 - acc: 0.4677
Epoch 61/100
62/62 [==============================] - 0s 291us/step - loss: 1.3808 - acc: 0.4516
Epoch 62/100
62/62 [==============================] - 0s 290us/step - loss: 1.3782 - acc: 0.4516
Epoch 63/100
62/62 [==============================] - 0s 306us/step - loss: 1.3496 - acc: 0.4516
Epoch 64/100
62/62 [==============================] - 0s 273us/step - loss: 1.3399 - acc: 0.4677
Epoch 65/100
62/62 [==============================] - 0s 290us/step - loss: 1.3420 - acc: 0.4677
Epoch 66/100
62/62 [==============================] - 0s 295us/step - loss: 1.3315 - acc: 0.4355
Epoch 67/100
62/62 [==============================] - 0s 306us/step - loss: 1.3320 - acc: 0.4355
Epoch 68/100
62/62 [==============================] - 0s 273us/step - loss: 1.3143 - acc: 0.4516
Epoch 69/100
62/62 [==============================] - 0s 308us/step - loss: 1.2953 - acc: 0.4516
Epoch 70/100
62/62 [==============================] - 0s 295us/step - loss: 1.2858 - acc: 0.4516
Epoch 71/100
62/62 [==============================] - 0s 309us/step - loss: 1.2975 - acc: 0.4516
Epoch 72/100
62/62 [==============================] - 0s 290us/step - loss: 1.2897 - acc: 0.4677
Epoch 73/100
62/62 [==============================] - 0s 289us/step - loss: 1.2496 - acc: 0.4677
Epoch 74/100
62/62 [==============================] - 0s 290us/step - loss: 1.2512 - acc: 0.4677
Epoch 75/100
62/62 [==============================] - 0s 276us/step - loss: 1.2379 - acc: 0.4677
Epoch 76/100
62/62 [==============================] - 0s 290us/step - loss: 1.2351 - acc: 0.5000
Epoch 77/100
62/62 [==============================] - 0s 296us/step - loss: 1.2140 - acc: 0.4839
Epoch 78/100
62/62 [==============================] - 0s 290us/step - loss: 1.2094 - acc: 0.5000
Epoch 79/100
62/62 [==============================] - 0s 273us/step - loss: 1.2008 - acc: 0.4839
Epoch 80/100
62/62 [==============================] - 0s 290us/step - loss: 1.1714 - acc: 0.5323
Epoch 81/100
62/62 [==============================] - 0s 305us/step - loss: 1.1626 - acc: 0.5161
Epoch 82/100
62/62 [==============================] - 0s 290us/step - loss: 1.1592 - acc: 0.5645
Epoch 83/100
62/62 [==============================] - 0s 304us/step - loss: 1.1355 - acc: 0.5323
Epoch 84/100
62/62 [==============================] - 0s 276us/step - loss: 1.1210 - acc: 0.5161
Epoch 85/100
62/62 [==============================] - 0s 325us/step - loss: 1.1573 - acc: 0.5000
Epoch 86/100
62/62 [==============================] - 0s 290us/step - loss: 1.1300 - acc: 0.5161
Epoch 87/100
62/62 [==============================] - 0s 306us/step - loss: 1.1085 - acc: 0.5323
Epoch 88/100
62/62 [==============================] - 0s 290us/step - loss: 1.1022 - acc: 0.5806
Epoch 89/100
62/62 [==============================] - 0s 306us/step - loss: 1.1110 - acc: 0.5806
Epoch 90/100
62/62 [==============================] - 0s 338us/step - loss: 1.0623 - acc: 0.5645
Epoch 91/100
62/62 [==============================] - 0s 290us/step - loss: 1.0652 - acc: 0.5968
Epoch 92/100
62/62 [==============================] - 0s 305us/step - loss: 1.0665 - acc: 0.5645
Epoch 93/100
62/62 [==============================] - 0s 279us/step - loss: 1.0654 - acc: 0.5968
Epoch 94/100
62/62 [==============================] - 0s 290us/step - loss: 1.0391 - acc: 0.6452
Epoch 95/100
62/62 [==============================] - 0s 322us/step - loss: 0.9968 - acc: 0.6774
Epoch 96/100
62/62 [==============================] - 0s 290us/step - loss: 1.0729 - acc: 0.5968
Epoch 97/100
62/62 [==============================] - 0s 290us/step - loss: 0.9876 - acc: 0.7097
Epoch 98/100
62/62 [==============================] - 0s 274us/step - loss: 0.9677 - acc: 0.7258
Epoch 99/100
62/62 [==============================] - 0s 306us/step - loss: 0.9735 - acc: 0.6935
Epoch 100/100
62/62 [==============================] - 0s 294us/step - loss: 0.9753 - acc: 0.6290
2019-04-08 20:31:16 INFO     rasa_core.policies.keras_policy  - Done fitting keras policy model
Processed actions: 62it [00:00, 2261.65it/s, # examples=62]
2019-04-08 20:31:17 INFO     rasa_core.agent  - Model directory models/dialogue exists and contains old model files. All files will be overwritten.
2019-04-08 20:31:17 INFO     rasa_core.agent  - Persisted model to 'C:\Users\Rohan Gore\Documents\Chatbot\rasa_core\models\dialogue'

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue
2019-04-08 20:33:42 INFO     root  - Rasa process starting
2019-04-08 20:33:52.510382: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 20:33:55 INFO     root  - Rasa Core server is up and running on http://localhost:5005
Bot loaded. Type a message and press enter (use '/stop' to exit):
Your input ->  /greet
127.0.0.1 - - [2019-04-08 20:34:02] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 185 0.281254
Hey! How are you?
Your input ->  fine
127.0.0.1 - - [2019-04-08 20:34:16] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.012931
Your input ->  /fine
127.0.0.1 - - [2019-04-08 20:34:26] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.012886
Your input ->  /greet
127.0.0.1 - - [2019-04-08 20:34:35] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.013924
Your input ->

Cancelled by user


(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_nlu.train -c nlu_config.yml --data nlu.md -o models --fixed_model_name nlu --project current --verbose
2019-04-08 20:35:32 INFO     rasa_nlu.utils.spacy_utils  - Trying to load spacy model with name 'en'
2019-04-08 20:36:02 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 20:36:03 INFO     rasa_nlu.training_data.loading  - Training data format of nlu.md is md
2019-04-08 20:36:03 INFO     rasa_nlu.training_data.training_data  - Training data stats:
        - intent examples: 39 (6 distinct intents)
        - Found intents: 'greet', 'mood_deny', 'mood_great', 'goodbye', 'mood_affirm', 'mood_unhappy'
        - entity examples: 0 (0 distinct entities)
        - found entities:

2019-04-08 20:36:03 INFO     rasa_nlu.model  - Starting to train component nlp_spacy
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Starting to train component tokenizer_spacy
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Starting to train component intent_featurizer_spacy
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Starting to train component intent_entity_featurizer_regex
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Starting to train component ner_crf
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Starting to train component ner_synonyms
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:04 INFO     rasa_nlu.model  - Starting to train component intent_classifier_sklearn
Fitting 2 folds for each of 6 candidates, totalling 12 fits
[Parallel(n_jobs=1)]: Using backend SequentialBackend with 1 concurrent workers.
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
[Parallel(n_jobs=1)]: Done  12 out of  12 | elapsed:    0.0s finished
2019-04-08 20:36:05 INFO     rasa_nlu.model  - Finished training component.
2019-04-08 20:36:05 INFO     rasa_nlu.model  - Successfully saved model into 'C:\Users\Rohan Gore\Documents\Chatbot\rasa_core\models\current\nlu'
2019-04-08 20:36:06 INFO     __main__  - Finished training

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu
2019-04-08 20:37:04 INFO     root  - Rasa process starting
2019-04-08 20:37:31 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 20:37:42.163807: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 20:37:45 INFO     root  - Rasa Core server is up and running on http://localhost:5005
Bot loaded. Type a message and press enter (use '/stop' to exit):
Your input ->  hi
Hey! How are you?127.0.0.1 - - [2019-04-08 20:37:50] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 185 0.288193

Your input ->  fine
127.0.0.1 - - [2019-04-08 20:37:57] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.038069
Your input ->  hi
127.0.0.1 - - [2019-04-08 20:38:01] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.036900
Your input ->  bye
127.0.0.1 - - [2019-04-08 20:38:05] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.035839
Your input ->

Cancelled by user


(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>rasa_core.run
'rasa_core.run' is not recognized as an internal or external command,
operable program or batch file.

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>--credentials credentials.yml
'--credentials' is not recognized as an internal or external command,
operable program or batch file.

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>rasa_core.run --credentials credentials.yml
'rasa_core.run' is not recognized as an internal or external command,
operable program or batch file.

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml
2019-04-08 21:25:13 INFO     root  - Rasa process starting
2019-04-08 21:25:40 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 21:25:51.246869: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 21:25:54 INFO     root  - Rasa Core server is up and running on http://localhost:5002
127.0.0.1 - - [2019-04-08 21:27:16] "GET / HTTP/1.1" 404 341 0.125352
127.0.0.1 - - [2019-04-08 21:27:16] "GET /favicon.ico HTTP/1.1" 404 341 0.001995
127.0.0.1 - - [2019-04-08 21:27:31] "GET / HTTP/1.1" 404 341 0.002030
127.0.0.1 - - [2019-04-08 21:29:30] "GET /webhooks/facebook/webhook?hub.mode=subscribe&hub.challenge=323967813&hub.verify_token=rasa-bot HTTP/1.1" 200 124 0.001056
2019-04-08 21:30:51 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 21:30:51] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.005032
127.0.0.1 - - [2019-04-08 21:30:52] "GET /favicon.ico HTTP/1.1" 404 341 0.001995
2019-04-08 21:31:14 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 21:31:14] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.003913
127.0.0.1 - - [2019-04-08 21:31:21] "GET / HTTP/1.1" 404 341 0.002074
2019-04-08 21:31:27 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 21:31:27] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.004190
2019-04-08 21:32:13 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 21:32:13] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.004945
127.0.0.1 - - [2019-04-08 21:32:25] "GET / HTTP/1.1" 404 341 0.000997
2019-04-08 21:32:46 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 21:32:46] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.003997
2019-04-08 22:29:43 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:29:43] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.007041
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:00:21Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml
2019-04-08 22:30:39 INFO     root  - Rasa process starting
2019-04-08 22:31:06 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:31:17.657106: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 22:31:20 INFO     root  - Rasa Core server is up and running on http://localhost:5002
2019-04-08 22:32:15 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:32:15] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.004048
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:09:39Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt
^C
(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -c facebook -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --debug
2019-04-08 22:40:27 INFO     root  - Rasa process starting
2019-04-08 22:40:54 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:41:05.340625: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 22:41:08 DEBUG    rasa_core.utils  - Available web server routes:
static                                             GET, OPTIONS, HEAD             /static/[filename]
fb_webhook.health                                  GET, OPTIONS, HEAD             /webhooks/facebook/
fb_webhook.webhook                                 OPTIONS, POST                  /webhooks/facebook/webhook
2019-04-08 22:41:08 INFO     root  - Rasa Core server is up and running on http://localhost:5002
127.0.0.1 - - [2019-04-08 22:41:39] "GET / HTTP/1.1" 404 341 0.001995
2019-04-08 22:41:46 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:41:46] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.004029
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:14:43Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml
2019-04-08 22:45:06 INFO     root  - Rasa process starting
2019-04-08 22:45:33 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:45:44.251629: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 22:45:47 INFO     root  - Rasa Core server is up and running on http://localhost:5002
2019-04-08 22:46:15 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:46:15] "GET /webhooks/facebook/webhook HTTP/1.1" 200 138 0.005054
127.0.0.1 - - [2019-04-08 22:46:34] "GET / HTTP/1.1" 404 341 0.003987
127.0.0.1 - - [2019-04-08 22:46:49] "GET / HTTP/1.1" 404 341 0.001641
127.0.0.1 - - [2019-04-08 22:47:18] "GET /o/webhooks/facebook/webhook HTTP/1.1" 404 341 0.001993
2019-04-08 22:47:34 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:47:34] "GET //webhooks/facebook/webhook HTTP/1.1" 200 138 0.004112
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:19:04Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/nlu/current \
usage: run.py [-h] -d CORE [-u NLU] [-p PORT] [--auth_token AUTH_TOKEN]
              [--cors [CORS [CORS ...]]] [-o LOG_FILE]
              [--credentials CREDENTIALS] [--endpoints ENDPOINTS]
              [-c CONNECTOR] [--enable_api] [--jwt_secret JWT_SECRET]
              [--jwt_method JWT_METHOD] [-v] [-vv] [--quiet]
run.py: error: unrecognized arguments: \

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/nlu/current --port 5002 --connector facebook --credentials fb_credentials.yml
2019-04-08 22:50:02 INFO     root  - Rasa process starting
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\model.py", line 74, in load
    data = utils.read_json_file(metadata_file)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\utils\__init__.py", line 212, in read_json_file
    content = read_file(filename)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\utils\__init__.py", line 206, in read_file
    with io.open(filename, encoding=encoding) as f:
FileNotFoundError: [Errno 2] No such file or directory: 'models/nlu/current\\metadata.json'

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 243, in <module>
    _endpoints.nlu)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\interpreter.py", line 31, in create
    return RasaNLUInterpreter(model_directory=obj)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\interpreter.py", line 231, in __init__
    self._load_interpreter()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\interpreter.py", line 247, in _load_interpreter
    self.interpreter = Interpreter.load(self.model_directory)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\model.py", line 288, in load
    model_metadata = Metadata.load(model_dir)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\model.py", line 79, in load
    "from '{}'. {}".format(abspath, e))
rasa_nlu.model.InvalidProjectError: Failed to load model metadata from 'C:\Users\Rohan Gore\Documents\Chatbot\rasa_core\models\nlu\current\metadata.json'. [Errno 2] No such file or directory: 'models/nlu/current\\metadata.json'

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --connector facebook --credentials fb_credentials.yml
2019-04-08 22:50:24 INFO     root  - Rasa process starting
2019-04-08 22:50:52 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:51:03.969517: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 190, in serve_application
    input_channels = create_http_input_channels(channel, credentials_file)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 103, in create_http_input_channels
    all_credentials = read_yaml_file(credentials_file)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\utils.py", line 316, in read_yaml_file
    return read_yaml_string(read_file(filename))
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\utils.py", line 356, in read_file
    with io.open(filename, encoding=encoding) as f:
FileNotFoundError: [Errno 2] No such file or directory: 'fb_credentials.yml'

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>echo "hi" > fb_credentials.yml

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --connector facebook --credentials fb_credentials.yml
2019-04-08 22:52:22 INFO     root  - Rasa process starting
2019-04-08 22:52:52 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:53:06.066001: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 190, in serve_application
    input_channels = create_http_input_channels(channel, credentials_file)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 108, in create_http_input_channels
    return [_create_single_channel(channel, all_credentials.get(channel))]
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 116, in _create_single_channel
    return BUILTIN_CHANNELS[channel].from_credentials(credentials)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\channels\facebook.py", line 207, in from_credentials
    cls.raise_missing_credentials_exception()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\channels\channel.py", line 142, in raise_missing_credentials_exception
    DOCS_BASE_URL, cls.name()))
Exception: To use the facebook input channel, you need to pass a credentials file using '--credentials'. The argument should be a file path pointing toa yml file containing the facebook authenticationinformation. Details in the docs: https://rasa.com/docs/core/connectors/#facebook-setup

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --connector facebook --credentials fb_credentials.yml
2019-04-08 22:55:13 INFO     root  - Rasa process starting
2019-04-08 22:55:40 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:55:51.673187: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 190, in serve_application
    input_channels = create_http_input_channels(channel, credentials_file)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 108, in create_http_input_channels
    return [_create_single_channel(channel, all_credentials.get(channel))]
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 116, in _create_single_channel
    return BUILTIN_CHANNELS[channel].from_credentials(credentials)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\channels\facebook.py", line 207, in from_credentials
    cls.raise_missing_credentials_exception()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\channels\channel.py", line 142, in raise_missing_credentials_exception
    DOCS_BASE_URL, cls.name()))
Exception: To use the facebook input channel, you need to pass a credentials file using '--credentials'. The argument should be a file path pointing toa yml file containing the facebook authenticationinformation. Details in the docs: https://rasa.com/docs/core/connectors/#facebook-setup

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --connector facebook --credentials fb_credentials.yml
2019-04-08 22:56:51 INFO     root  - Rasa process starting
2019-04-08 22:57:18 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 22:57:29.367198: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 22:57:32 INFO     root  - Rasa Core server is up and running on http://localhost:5002
2019-04-08 22:57:50 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:57:50] "GET //webhooks/facebook/webhook HTTP/1.1" 200 138 0.005228
2019-04-08 22:57:54 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 22:57:54] "GET //webhooks/facebook/webhook HTTP/1.1" 200 138 0.005134
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:34:17Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/nlu/current --port 5002 --connector facebook --credentials fb_credentials.yml --enable_api
2019-04-08 23:05:54 INFO     root  - Rasa process starting
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\model.py", line 74, in load
    data = utils.read_json_file(metadata_file)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\utils\__init__.py", line 212, in read_json_file
    content = read_file(filename)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\utils\__init__.py", line 206, in read_file
    with io.open(filename, encoding=encoding) as f:
FileNotFoundError: [Errno 2] No such file or directory: 'models/nlu/current\\metadata.json'

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 243, in <module>
    _endpoints.nlu)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\interpreter.py", line 31, in create
    return RasaNLUInterpreter(model_directory=obj)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\interpreter.py", line 231, in __init__
    self._load_interpreter()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\interpreter.py", line 247, in _load_interpreter
    self.interpreter = Interpreter.load(self.model_directory)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\model.py", line 288, in load
    model_metadata = Metadata.load(model_dir)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_nlu\model.py", line 79, in load
    "from '{}'. {}".format(abspath, e))
rasa_nlu.model.InvalidProjectError: Failed to load model metadata from 'C:\Users\Rohan Gore\Documents\Chatbot\rasa_core\models\nlu\current\metadata.json'. [Errno 2] No such file or directory: 'models/nlu/current\\metadata.json'

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --connector facebook --credentials fb_credentials.yml --enable_api
2019-04-08 23:06:31 INFO     root  - Rasa process starting
2019-04-08 23:07:00 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 23:07:13.169200: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 23:07:16 INFO     root  - Rasa Core server is up and running on http://localhost:5002
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:40:49Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --connector facebook --credentials fb_credentials.yml --enable_api --debug
2019-04-08 23:11:43 INFO     root  - Rasa process starting
2019-04-08 23:12:11 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 23:12:24.288332: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 23:12:27 DEBUG    rasa_core.utils  - Available web server routes:
hello                                              GET, HEAD, OPTIONS             /
list_trackers                                      GET, HEAD, OPTIONS             /conversations
execute_action                                     POST, OPTIONS                  /conversations/[sender_id]/execute
log_message                                        POST, OPTIONS                  /conversations/[sender_id]/messages
predict                                            POST, OPTIONS                  /conversations/[sender_id]/predict
respond                                            GET, POST, OPTIONS, HEAD       /conversations/[sender_id]/respond
retrieve_story                                     GET, HEAD, OPTIONS             /conversations/[sender_id]/story
retrieve_tracker                                   GET, HEAD, OPTIONS             /conversations/[sender_id]/tracker
replace_events                                     PUT, OPTIONS                   /conversations/[sender_id]/tracker/events
get_domain                                         GET, HEAD, OPTIONS             /domain
evaluate_stories                                   POST, OPTIONS                  /evaluate
continue_training                                  POST, OPTIONS                  /finetune
load_model                                         POST, OPTIONS                  /model
tracker_predict                                    POST, OPTIONS                  /predict
static                                             GET, HEAD, OPTIONS             /static/[filename]
status                                             GET, HEAD, OPTIONS             /status
version                                            GET, HEAD, OPTIONS             /version
fb_webhook.health                                  GET, HEAD, OPTIONS             /webhooks/facebook/
fb_webhook.webhook                                 POST, OPTIONS                  /webhooks/facebook/webhook
2019-04-08 23:12:27 INFO     root  - Rasa Core server is up and running on http://localhost:5002
127.0.0.1 - - [2019-04-08 23:13:01] "GET / HTTP/1.1" 200 144 0.001931
127.0.0.1 - - [2019-04-08 23:13:51] "GET / HTTP/1.1" 200 144 0.001983
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T17:47:47Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --enable_api

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --enable_api --debug
2019-04-08 23:19:07 INFO     root  - Rasa process starting
2019-04-08 23:19:36 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-08 23:19:49.168605: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-08 23:19:52 DEBUG    rasa_core.utils  - Available web server routes:
hello                                              GET, OPTIONS, HEAD             /
list_trackers                                      GET, OPTIONS, HEAD             /conversations
execute_action                                     POST, OPTIONS                  /conversations/[sender_id]/execute
log_message                                        POST, OPTIONS                  /conversations/[sender_id]/messages
predict                                            POST, OPTIONS                  /conversations/[sender_id]/predict
respond                                            GET, OPTIONS, POST, HEAD       /conversations/[sender_id]/respond
retrieve_story                                     GET, OPTIONS, HEAD             /conversations/[sender_id]/story
retrieve_tracker                                   GET, OPTIONS, HEAD             /conversations/[sender_id]/tracker
replace_events                                     OPTIONS, PUT                   /conversations/[sender_id]/tracker/events
get_domain                                         GET, OPTIONS, HEAD             /domain
evaluate_stories                                   POST, OPTIONS                  /evaluate
continue_training                                  POST, OPTIONS                  /finetune
load_model                                         POST, OPTIONS                  /model
tracker_predict                                    POST, OPTIONS                  /predict
static                                             GET, OPTIONS, HEAD             /static/[filename]
status                                             GET, OPTIONS, HEAD             /status
version                                            GET, OPTIONS, HEAD             /version
fb_webhook.health                                  GET, OPTIONS, HEAD             /webhooks/facebook/
fb_webhook.webhook                                 POST, OPTIONS                  /webhooks/facebook/webhook
2019-04-08 23:19:52 INFO     root  - Rasa Core server is up and running on http://localhost:5002
127.0.0.1 - - [2019-04-08 23:24:16] "GET /webhooks/facebook/webhook?hub.mode=subscribe&hub.challenge=986374459&hub.verify_token=rasa-bot HTTP/1.1" 200 156 0.002036
127.0.0.1 - - [2019-04-08 23:26:32] "GET / HTTP/1.1" 200 144 0.002137
127.0.0.1 - - [2019-04-08 23:26:33] "GET /favicon.ico HTTP/1.1" 404 373 0.000997
2019-04-08 23:27:36 WARNING  rasa_core.channels.facebook  - Invalid fb verify token! Make sure this matches your webhook settings on the facebook app.
127.0.0.1 - - [2019-04-08 23:27:36] "GET /webhooks/facebook/webhook HTTP/1.1" 200 170 0.006149
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T18:32:48Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_nlu.train -c nlu_config.yml --data nlu.md -o models --fixed_model_name nlu --project current --verbose
2019-04-09 00:18:17 INFO     rasa_nlu.utils.spacy_utils  - Trying to load spacy model with name 'en'
2019-04-09 00:18:42 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-09 00:18:42 INFO     rasa_nlu.training_data.loading  - Training data format of nlu.md is md
2019-04-09 00:18:42 INFO     rasa_nlu.training_data.training_data  - Training data stats:
        - intent examples: 39 (6 distinct intents)
        - Found intents: 'mood_great', 'greet', 'mood_affirm', 'mood_deny', 'goodbye', 'mood_unhappy'
        - entity examples: 0 (0 distinct entities)
        - found entities:

2019-04-09 00:18:42 INFO     rasa_nlu.model  - Starting to train component nlp_spacy
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Starting to train component tokenizer_spacy
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Starting to train component intent_featurizer_spacy
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Starting to train component intent_entity_featurizer_regex
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Starting to train component ner_crf
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Starting to train component ner_synonyms
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:43 INFO     rasa_nlu.model  - Starting to train component intent_classifier_sklearn
Fitting 2 folds for each of 6 candidates, totalling 12 fits
[Parallel(n_jobs=1)]: Using backend SequentialBackend with 1 concurrent workers.
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
[Parallel(n_jobs=1)]: Done  12 out of  12 | elapsed:    0.1s finished
2019-04-09 00:18:44 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:18:44 INFO     rasa_nlu.model  - Successfully saved model into 'C:\Users\Rohan Gore\Documents\Chatbot\rasa_core\models\current\nlu'
2019-04-09 00:18:45 INFO     __main__  - Finished training

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue
2019-04-09 00:19:09 INFO     root  - Rasa process starting
2019-04-09 00:19:19.907491: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-09 00:19:22 INFO     root  - Rasa Core server is up and running on http://localhost:5005
Bot loaded. Type a message and press enter (use '/stop' to exit):
Your input ->  hi
127.0.0.1 - - [2019-04-09 00:19:29] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.302158
Your input ->  /greet
Hey! How are you?
127.0.0.1 - - [2019-04-09 00:19:33] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 185 0.015920
Your input ->

Cancelled by user


(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_nlu.train -c nlu_config.yml --data nlu.md -o models --fixed_model_name nlu --project current --verbose
2019-04-09 00:20:27 INFO     rasa_nlu.utils.spacy_utils  - Trying to load spacy model with name 'en'
2019-04-09 00:20:54 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-09 00:20:54 INFO     rasa_nlu.training_data.loading  - Training data format of nlu.md is md
2019-04-09 00:20:54 INFO     rasa_nlu.training_data.training_data  - Training data stats:
        - intent examples: 39 (6 distinct intents)
        - Found intents: 'greet', 'mood_affirm', 'mood_great', 'mood_deny', 'mood_unhappy', 'goodbye'
        - entity examples: 0 (0 distinct entities)
        - found entities:

2019-04-09 00:20:54 INFO     rasa_nlu.model  - Starting to train component nlp_spacy
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Starting to train component tokenizer_spacy
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Starting to train component intent_featurizer_spacy
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Starting to train component intent_entity_featurizer_regex
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Starting to train component ner_crf
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Starting to train component ner_synonyms
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:55 INFO     rasa_nlu.model  - Starting to train component intent_classifier_sklearn
Fitting 2 folds for each of 6 candidates, totalling 12 fits
[Parallel(n_jobs=1)]: Using backend SequentialBackend with 1 concurrent workers.
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\sklearn\metrics\classification.py:1143: UndefinedMetricWarning: F-score is ill-defined and being set to 0.0 in labels with no predicted samples.
  'precision', 'predicted', average, warn_for)
[Parallel(n_jobs=1)]: Done  12 out of  12 | elapsed:    0.0s finished
2019-04-09 00:20:56 INFO     rasa_nlu.model  - Finished training component.
2019-04-09 00:20:56 INFO     rasa_nlu.model  - Successfully saved model into 'C:\Users\Rohan Gore\Documents\Chatbot\rasa_core\models\current\nlu'
2019-04-09 00:20:56 INFO     __main__  - Finished training

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu
2019-04-09 00:23:45 INFO     root  - Rasa process starting
2019-04-09 00:24:10 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-09 00:24:21.073288: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-09 00:24:23 INFO     root  - Rasa Core server is up and running on http://localhost:5005
Bot loaded. Type a message and press enter (use '/stop' to exit):
Your input ->  hi
Hey! How are you?
127.0.0.1 - - [2019-04-09 00:25:06] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 185 0.252360
Your input ->  fine
127.0.0.1 - - [2019-04-09 00:25:10] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.030881
Your input ->  hi
127.0.0.1 - - [2019-04-09 00:25:16] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.036902
Your input ->

Cancelled by user


(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu
2019-04-09 00:26:07 INFO     root  - Rasa process starting
2019-04-09 00:26:33 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-09 00:29:30.996612: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-09 00:29:33 INFO     root  - Rasa Core server is up and running on http://localhost:5005
Bot loaded. Type a message and press enter (use '/stop' to exit):
Your input ->
127.0.0.1 - - [2019-04-09 00:29:35] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 122 0.237399
Your input ->  hi
Hey! How are you?
127.0.0.1 - - [2019-04-09 00:29:44] "POST /webhooks/rest/webhook?stream=true&token= HTTP/1.1" 200 185 0.035866
Your input ->

Cancelled by user


(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml
2019-04-09 00:30:15 INFO     root  - Rasa process starting
2019-04-09 00:30:42 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-09 00:30:52.807965: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-09 00:30:55 INFO     root  - Rasa Core server is up and running on http://localhost:5002
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\_ffi\loop.py", line 234, in python_check_callback
    def python_check_callback(self, watcher_ptr): # pylint:disable=unused-argument
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\engineio\client.py", line 41, in signal_handler
    return original_signal_handler(sig, frame)
KeyboardInterrupt
2019-04-08T19:00:59Z
Traceback (most recent call last):
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 193, in _run_module_as_main
    "__main__", mod_spec)
  File "C:\Users\Rohan Gore\Anaconda3\lib\runpy.py", line 85, in _run_code
    exec(code, run_globals)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 260, in <module>
    cmdline_args.jwt_method)
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\rasa_core\run.py", line 201, in serve_application
    http_server.serve_forever()
  File "C:\Users\Rohan Gore\Documents\Chatbot\rasabot\lib\site-packages\gevent\baseserver.py", line 369, in serve_forever
    self._stop_event.wait()
  File "src\gevent\event.py", line 127, in gevent._event.Event.wait
  File "src\gevent\_abstract_linkable.py", line 192, in gevent.__abstract_linkable.AbstractLinkable._wait
  File "src\gevent\_abstract_linkable.py", line 165, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_abstract_linkable.py", line 169, in gevent.__abstract_linkable.AbstractLinkable._wait_core
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 60, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\_greenlet_primitives.py", line 64, in gevent.__greenlet_primitives.SwitchOutGreenletWithLoop.switch
  File "src\gevent\__greenlet_primitives.pxd", line 35, in gevent.__greenlet_primitives._greenlet_switch
KeyboardInterrupt

(rasabot) C:\Users\Rohan Gore\Documents\Chatbot\rasa_core>python -m rasa_core.run -d models/dialogue -u models/current/nlu --port 5002 --credentials credentials.yml --enable_api --debug
2019-04-09 00:31:33 INFO     root  - Rasa process starting
2019-04-09 00:31:59 INFO     rasa_nlu.components  - Added 'nlp_spacy' to component cache. Key 'nlp_spacy-en'.
2019-04-09 00:32:09.117266: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2
2019-04-09 00:32:11 DEBUG    rasa_core.utils  - Available web server routes:
hello                                              OPTIONS, GET, HEAD             /
list_trackers                                      OPTIONS, GET, HEAD             /conversations
execute_action                                     OPTIONS, POST                  /conversations/[sender_id]/execute
log_message                                        OPTIONS, POST                  /conversations/[sender_id]/messages
predict                                            OPTIONS, POST                  /conversations/[sender_id]/predict
respond                                            OPTIONS, POST, HEAD, GET       /conversations/[sender_id]/respond
retrieve_story                                     OPTIONS, GET, HEAD             /conversations/[sender_id]/story
retrieve_tracker                                   OPTIONS, GET, HEAD             /conversations/[sender_id]/tracker
replace_events                                     OPTIONS, PUT                   /conversations/[sender_id]/tracker/events
get_domain                                         OPTIONS, GET, HEAD             /domain
evaluate_stories                                   OPTIONS, POST                  /evaluate
continue_training                                  OPTIONS, POST                  /finetune
load_model                                         OPTIONS, POST                  /model
tracker_predict                                    OPTIONS, POST                  /predict
static                                             OPTIONS, GET, HEAD             /static/[filename]
status                                             OPTIONS, GET, HEAD             /status
version                                            OPTIONS, GET, HEAD             /version
fb_webhook.health                                  OPTIONS, GET, HEAD             /webhooks/facebook/
fb_webhook.webhook                                 OPTIONS, POST                  /webhooks/facebook/webhook
2019-04-09 00:32:11 INFO     root  - Rasa Core server is up and running on http://localhost:5002
