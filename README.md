# seq2seq-chatbot
A sequence2sequence chatbot implementation with TensorFlow.

The models and datsets are uploaded in google drive due to size issues.

## Chatting with a trained model
To chat with a trained model from a python console:

1. Set console working directory to the **seq2seq-chatbot** directory. This directory should have the **models** and **datasets** directories directly within it.

2. Run chat.py with the model checkpoint path:
```shell
run chat.py models\dataset_name\model_name\checkpoint.ckpt
```
