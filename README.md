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

For example, to chat with the trained cornell movie dialog model **trained_model_v1**:

1. Download and unzip [trained_model_v1](seq2seq-chatbot/models/cornell_movie_dialog/README.md) into the [seq2seq-chatbot/models/cornell_movie_dialog](seq2seq-chatbot/models/cornell_movie_dialog) folder

2. Set console working directory to the **seq2seq-chatbot** directory

3. Run:
```shell
run chat.py models\cornell_movie_dialog\trained_model_v1\best_weights_training.ckpt
```

The result should look like this:

![chat](doc_files/chat.png "chat")

## Training a model
To train a model from a python console:

1. Configure the [hparams.json](seq2seq-chatbot/hparams.json) file to the desired training hyperparameters

2. Set console working directory to the **seq2seq-chatbot** directory. This directory should have the **models** and **datasets** directories directly within it.

3. To train a new model, run train.py with the dataset path:
```shell
run train.py --datasetdir=datasets\dataset_name
```

Or to resume training an existing model, run train.py with the model checkpoint path:
```shell
run train.py --checkpointfile=models\dataset_name\model_name\checkpoint.ckpt
```

For example, to train a new model on the cornell movie dialog dataset with default hyperparameters:

1. Set console working directory to the **seq2seq-chatbot** directory

2. Run:
```shell
run train.py --datasetdir=datasets\cornell_movie_dialog
```
