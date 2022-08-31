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

For example, to chat with the trained question & answer model **trained_model_v1**:

1. Download and unzip [trained_model_v1](seq2seq-chatbot/models/question&answer/README.md) into the [seq2seq-chatbot/models/question&answer](seq2seq-chatbot/models/question&answer) folder

2. Set console working directory to the **seq2seq-chatbot** directory

3. Run:
```shell
run chat.py models\question&answer\trained_model_v1\best_weights_training.ckpt
```
