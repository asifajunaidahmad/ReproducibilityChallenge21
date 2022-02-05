# ReproducibilityChallenge21
This folder contains complete code to reproduce FakeFlow model
FakeFlow: Fake News Detection by Modeling the Flow of Affective Information
The Code work on only below specific versions and Libraries

**REQUIREMENTS**

gensim==3.8.0 <br />
joblib==0.14.1 <br />
Keras==2.2.4 <br />
Keras-Preprocessing==1.1.0 <br />
keras-self-attention==0.35.0 <br />
numpy==1.16.0 <br />
pandas==0.24.2 <br />
nltk==3.4.5 <br />
scikit-learn==0.20.2 <br />
tensorflow-gpu==1.14.0 <br />
tqdm==4.32.1 <br />
hyperopt==0.1.1 <br />
Place your data in the folder ./data/shffufle_data.csv <br />
To run the model, run the file: work.ipynb  <br />
parameters: -d: dataset name (i.e. shuffle_data.csv).

-sn: number of segments. <br />

-s: to search for params; enter a number larger than 0 to search for N different combination of parameters (e.g. 150). <br />

-m: mode (train or test); if you want to load a pretrained model. <br />
An example: <br />

work.ipynb -d MultiSourceFake -sn 10 <br />

To load saved model after training: <br />

work.ipynb  -d MultiSourceFake -sn 10 -m test <br />

To search for best params: <br />

work.ipynb -d MultiSourceFake -s 80 <br />
