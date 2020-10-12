# Neural Networks

## Goal
In this project, I'm building a neural network to predict whether or not a student is paying attention, based on data of webcam images.

## Tasks

* Explain the utility of artificial neural networks
* Explain the backpropagation algorithm
* Build a basic neural network to solve a prediction problem

## Data
The attached data sets attention1.csv and attention2.csv provide features assocaited with webcam images of 100 students' faces as they particpate in an online discussion. The variables are:

eyes - student has their eyes open (1 = yes, 0 = no)
face.forward - student is facing the camera (1 = yes, 0 = no)
chin.up - student's chin is raised above 45 degrees (1 = yes, 0 = no)
attention - whether the student was paying attention when asked (1 = yes, 0 = no)

## Procedures
* Build a neural network containing one hidden layer
* Add a hidden layer and compare the two networks
* Use the better one to make predictions
* Draw conclusions from the predictions

## Required Packages
```
install.packages("neuralnet")
```

## Background
Neural networks are not a new method, the first artificial neural network was devised in 1943, but advances in computational power and speed have made them a much more viable strategy for solving complex problems over the last 5-10 years. Originally devised by mathmaticians and neuroscientists to illustrate the fundamental principles of how brains might work they lost favor in the second half of the 20th century only to surge in popularity in the 20-teens as software engineers used them to resolve mathmatically intractable problems. The application of neural networks to learning problems has been ongoing for 20 years, often to predict student behvior or to parse unstructured data such as student writing samples and provide natural sounding feedback through AI avatars.

### Brief Introduction to Concepts
**Neurons** or **nodes** is a loose analogy to biological neurons. They are processors of information that lead us to the output. Each neuron is connected with another neuron through a link. Each link is specified by a weight and a bias.
The **input layer** accepts independent variables or our input of data; they are then passed through to **hidden layers** and eventually the **output layer**, which generates predictions.
Each time we feed input information to the network, it generates a predicted output, with which we compare the target output we want. The difference between the prediction and the target is the **cost**. By feeding a large amount of cases into the network, we arrive at the weights and biases parameters that would minimize the average costs. **Gradient descendent** is calculated and used to make these adjustments. Commonly, training data are randomly divided into small batches to generate approximate descendents more quickly, referred to as stochastic gradient descendents, to speed up the process. 
**Back propogation** is the algorithm for determining how a single training example would modify the weights and biases.

##  References

Nielsen, M. (2015). Neural Networks & Deep Learning. Determination Press:San Francisco, CA  
  [Chapter 1](http://neuralnetworksanddeeplearning.com/chap1.html)  
  [Charpter 2](http://neuralnetworksanddeeplearning.com/chap2.html)  

[McKlin, T., Harmon, S. W., Evans, W., & Jones, M. G. (2001). Cognitive presence in Web-based learning: A content analysis of students' online discussions.](https://files.eric.ed.gov/fulltext/ED470101.pdf)  

[Stergiou, C. & Siganos, D. (2000). Neural Networks.](http://www.doc.ic.ac.uk/~nd/surprise_96/journal/vol4/cs11/report.html)

[Hartnett, K. (2019). Foundations Built for a General Theory of Neural Networks](https://www.quantamagazine.org/foundations-built-for-a-general-theory-of-neural-networks-20190131/)

[Sanderson, G. (2017). But what *is* a Neural Network? 3Blue1Brown. ](https://www.youtube.com/watch?v=aircAruvnKk)

[Grey, C.G.P. (2017). How Machines Learn.](https://www.youtube.com/watch?v=R9OHn5ZF4Uo)

[Bling, S. (2017). MariFlow - Self-Driving Mario Kart with Recurrent Neural Network](https://www.youtube.com/watch?v=Ipi40cb_RsI)