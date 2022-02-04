# ReproducibilityChallenge21
This folder contains complete code to reproduce FakeFlow model
FakeFlow: Fake News Detection by Modeling the Flow of Affective Information
The Code work on only below specific versions and Libraries
REQUIREMENTS
gensim==3.8.0
joblib==0.14.1
Keras==2.2.4
Keras-Preprocessing==1.1.0
keras-self-attention==0.35.0
numpy==1.16.0
pandas==0.24.2
nltk==3.4.5
scikit-learn==0.20.2
tensorflow-gpu==1.14.0
tqdm==4.32.1
hyperopt==0.1.1
Place your data in the folder ./data/DATASET_NAME
To run the model, run the file: work.ipynb
parameters: -d: dataset name (i.e. MultiSourceFake).

-sn: number of segments.

-s: to search for params; enter a number larger than 0 to search for N different combination of parameters (e.g. 150).

-m: mode (train or test); if you want to load a pretrained model.
An example:

work.ipynb -d MultiSourceFake -sn 10

To load saved model after training:

work.ipynb  -d MultiSourceFake -sn 10 -m test

To search for best params:

work.ipynb -d MultiSourceFake -s 80
