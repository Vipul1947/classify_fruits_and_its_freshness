<h1> Classify fruits and check their freshness </h1>
 
<h2> Description</h2>

I had made an interactive web app so as to classify fruits into :

- Apple
- Banana
- Orange
<br>
Also it tells whether the fruit is fresh/rotten and to implement this webapp we had used Flask (a framework of Python), which uses a convolution neural network on the back end to perform the above classification.
<br>
<h2> LIVE LINK : https://classify-fresh-fruit-by-vipul.herokuapp.com/ </h2>
<br>
 <h2>Model</h2>

![image](https://user-images.githubusercontent.com/56962974/133897425-400dd6d8-234a-448e-bcc5-342841dd7c27.png)


The network itself was implemented using **transfer learning**. The MobileNet V2 model developed at Google was used as a base model for feature extraction from our data. A custom classification layer was added on top and trained separately. You can learn more about this approach [here](https://www.tensorflow.org/tutorials/images/transfer_learning). The notebook I used to implement the model on Google Colab can be found [here](https://github.com/Vipul1947/classify_fruits_and_its_freshness/blob/main/notebooks/FruitNetTransferLearning.ipynb).
<br><br>
<h2> Dataset for training</h2>
The dataset used for training and evaluating the model: (https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification). The obtained model has achieved 99% accuracy on the test set.
<br>
<br>
<h2> FLOW CHART </h2>

![WhatsApp Image 2021-09-13 at 16 21 11](https://user-images.githubusercontent.com/56962974/133897832-ea2f6ef3-ec47-44fc-a366-390243b37f3e.jpeg)


<br>
<h2> Dependencies</h2>

For this project, the following tools were used:
- [Tensorflow 2](https://www.tensorflow.org/install) for building and training the model
- [Numpy](https://numpy.org/) for working with arrays
- [Matplotlib](https://matplotlib.org/) for visualizing the data
- [Flask](https://flask.palletsprojects.com/en/1.1.x/) for implementing the server side
- HTML5, CSS3, JavaScript (with Web Speech API and [particles.js](https://vincentgarreau.com/particles.js/)) on the front-end.
<br><br>
<h2>IO Screenshots</h2>

![image](https://user-images.githubusercontent.com/56962974/133897974-31c52135-4a5b-4077-9856-fbd41cdc7563.png)

![image](https://user-images.githubusercontent.com/56962974/133898037-64a3540b-5ec3-4bd5-8487-e8122d7dba50.png)

![image](https://user-images.githubusercontent.com/56962974/133898085-a94be700-06a2-42f3-89fc-eaf3143ed011.png)

<br>

<h2> Install and run on local host</h2>

<h4>To install and run local host:</h4>

```bash
git clone https://github.com/Vipul1947/classify_fruits_and_its_freshness.git
cd classify_fruits_and_its_freshness
pip install -r requirements.txt
python app.py
```
