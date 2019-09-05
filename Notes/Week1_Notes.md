
## Week01 Basic Concept and Linear Regression(1)

### Basic concept

Many scientists think the best way to make progress on this is through learning algorithms called neural networks, which mimic how the human brain works.  
A computer program is said to:  
> "Learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experience E."  

In general, any machine learning problem can be assigned to one of two broad classifications:  
Supervised learning and Unsupervised learning.  
- **Supervised learning** :  
 1. Regression problem. eg: house price forecast (quadratic function is better)  
 2. Classification problem. eg: malignant tumor judgment 0/1  
*regression problem* could be converted to *classification problem*, such like *the price forecast* is converted into *whether it is sold*.  
- **Unsupervised learning** :  
Given a bunch of data without the so-called "correct answer" for automatic classification. Such as *Social network analysis*, *Market segmentation*, *Celestial data analysis*  
 1. Clustering problem. eg: genomic classification problems  
 2. Non-clustering problem. eg: audio noise process

### Linear Regression

#### Model and Cost Function

To describe the supervised learning problem slightly more formally, our goal is, given a training set, to learn a function $h : X → Y$ so that $h(x)$ is a “good” predictor for the corresponding value of $y$. For historical reasons, this function $h$ is called a *hypothesis*. Seen pictorially, the process is therefore like this:  
 <img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/notes/Imgs/week1_flow.png" width = "350" height = "250" alt="" align=center />  
We can measure the accuracy of our hypothesis function by using a **cost function**  
 <img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2013.30.08.png" width = "450" height = "350" alt="" align=center />  
If only consider $\theta_1$ where $\theta_0 = 0$, we could draw a $y - x$ line and a two-dimensional $J - \theta_1$ graph:  
 <img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2013.30.21.png" width = "500" height = "400" alt="" align=center />  
If consider two variable parameters $\theta_0$ and $\theta_1$, it's changed to a three-dimensional graph (or two-dimensional contuor graph):  
 <img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2013.30.32.png" width = "500" height = "400" alt="" align=center />  


#### Parameter Learning of Model

##### Gradient Descent algorithm

One of the features of Gradient Descent algorithm: Different starting points may get different <u>local</u> optimal solutions.  
<img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2018.49.21.png" width = "450" height = "350" alt="" align=center />  
**Note:** Execute simultaneously.  
The size of each step is determined by the parameter $\alpha$, which is called the *learning rate*. If $\alpha$ too small or too big, it would cause the convergence time to be too long or unable to converge.   
<img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2018.49.50.png" width = "400" height = "300" alt="" align=center /><img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2018.50.00.png" width = "400" height = "300" alt="" align=center />  

#### Summary
<img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2019.00.48.png" width = "500" height = "400" alt="" align=center />  
Integrated linear recursive algorithm:  
<img src="https://raw.githubusercontent.com/QQQingyu/AndrewNg-ML-Learn/master/Imgs/Week1_courseslide%202019-09-05%20at%2018.52.47.png" width = "500" height = "400" alt="" align=center />  

