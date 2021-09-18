# Classify fruits and check their freshness 

## Description

I had made an interactive web app so as to classify fruits into :-<br>
1.) Apple<br>
2.) Banana <br>
3.) Orange<br>
Also it tells whether the fruit is fresh/rotten and to implement this webapp we had used Flask (a framework of Python), which uses a convolution neural network on the back end to perform the above classification.
<br>
<br>
# **LIVE LINK :** https://classify-fresh-fruit-by-vipul.herokuapp.com/
<br>
<br>
## Model
![image](https://user-images.githubusercontent.com/56962974/133896624-ed0c4e30-785a-48dc-a008-c4d525da892e.png)
<br>
The network itself was implemented using **transfer learning**. The MobileNet V2 model developed at Google was used as a base model for feature extraction from our data. A custom classification layer was added on top and trained separately. You can learn more about this approach [here](https://www.tensorflow.org/tutorials/images/transfer_learning). The notebook I used to implement the model on Google Colab can be found [here](https://github.com/Vipul1947/classify_fruits_and_its_freshness/blob/main/notebooks/FruitNetTransferLearning.ipynb).
<br><br>
### Dependencies
For this project, the following tools were used:
- [Tensorflow 2](https://www.tensorflow.org/install) for building and training the model;
- [Numpy](https://numpy.org/) for working with arrays;
- [Matplotlib](https://matplotlib.org/) for visualizing the data;
- [Flask](https://flask.palletsprojects.com/en/1.1.x/) for implementing the server side;
- HTML5, CSS3, JavaScript (with Web Speech API and [particles.js](https://vincentgarreau.com/particles.js/)) on the front-end.
<br>
### Dataset for training
<br>
The dataset used for training and evaluating the model: (https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification) by Sriram Reddy Kalluri. The obtained model has achieved 99% accuracy on the test set.
<br>
<br>
## Install and Run in local host :
<br>
To install and run locally in local host :
```bash
git clone https://github.com/Vipul1947/classify_fruits_and_its_freshness.git
cd classify_fruits_and_its_freshness
pip install -r requirements.txt
python app.py
```
