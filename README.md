# Classify fruits and check their freshness 

## Description

I had made an interactive web app so as to classify fruits into :-
1.) Apple
2.) Banana 
3.) Orange
Also it tells whether the fruit is fresh/rotten and to implement this webapp we had used Flask (a framework of Python), which uses a convolution neural network on the back end to perform the above classification.


**The application is available at:** https://classify-fresh-fruit-by-vipul.herokuapp.com/

### Dependencies

For this project, the following tools were used:
- [Tensorflow 2](https://www.tensorflow.org/install) for building and training the model;
- [Numpy](https://numpy.org/) for working with arrays;
- [Matplotlib](https://matplotlib.org/) for visualizing the data;
- [Flask](https://flask.palletsprojects.com/en/1.1.x/) for implementing the server side;
- HTML5, CSS3, JavaScript (with Web Speech API and [particles.js](https://vincentgarreau.com/particles.js/)) on the front-end.

### Dataset for training

The dataset used for training and evaluating the model: [Fruits fresh and rotten for classification](https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification) by Sriram Reddy Kalluri. The obtained model has achieved 99% accuracy on the test set.

### Network implementation

The network itself was implemented using **transfer learning**. The MobileNet V2 model developed at Google was used as a base model for feature extraction from our data. A custom classification layer was added on top and trained separately. You can learn more about this approach [here](https://www.tensorflow.org/tutorials/images/transfer_learning). The notebook I used to implement the model on Google Colab can be found [here](https://github.com/AlexanderKlanovets/fruitnet/blob/master/notebooks/FruitNetTransferLearning.ipynb).

## Install locally

To install and run locally in a production mode:

```bash
git clone https://github.com/AlexanderKlanovets/fruitnet
cd fruitnet
pip install -r requirements.txt
python app.py
```

Another way is to run the app with Docker:
```bash
git clone https://github.com/AlexanderKlanovets/fruitnet
cd fruitnet
sudo docker build -t <image_name> .
sudo docker run -p 5000:5000 <image_name>
```
