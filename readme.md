# Gradient Descent Algorithm

Gradient descent (GD) is an iterative first-order optimisation algorithm used to find a local minimum/maximum of a given function. This method is commonly used in machine learning (ML) and deep learning(DL) to minimise a cost/loss function (e.g. in a linear regression).

To understand the Gradient Descent Algorithm let us consider a Simple Linear Regression problem, for given CGPA of the student and we need to predict the package(lpa) he/she cracked.

* step 1: Gathered the student placement data.
* step 2: Train the Linear Regression model with the data.

![dataset plot](https://user-images.githubusercontent.com/37456341/158873842-d88373a1-a6d2-4cd6-b0b6-e070fa5afa4f.png)


As data is sort of linearly distributed so we need to find out the best fit line.

#### line equation: y=m*x + b

      m=slope of line
      
      b=y-intercept of line

#### For given problem equation is: package = m * CGPA + b

So during the training of the model we need to find out the values of m and b w.r.t best fit line.

Here th Gradient Descent algorithm comes into the picture which helps us to evaluate the values of m and b for the best fit line(i.e a line with minimum loss/cost).

## Gradient Descent Algorithm

* choose a starting point (initialisation)

* calculate gradient at this point

* make a scaled step in the opposite direction to the gradient (objective: minimise)

* repeat points 2 and 3 until one of the criteria is met:

      * maximum number of iterations reached
      * step size is smaller than the tolerance.


## Cost function converge to minima. 

Cost function value converging to minimum value as the number of iterations increasing.
![2) gd algo](https://user-images.githubusercontent.com/37456341/158860140-67475a8d-fe71-44aa-a2be-c7bb082e20ab.gif)

## Getting best fit line

As the cost function value converge to minima the line(initialize with random m and b values) tends to best fit to line.
![1) best fit line](https://user-images.githubusercontent.com/37456341/158859589-be43fcb1-e0cf-4051-a108-42e0b49256e4.gif)


## y-intercept(b) V/S epochs plot

* Intially the intercept value is decreasing with iterations.
* After some iterations the change in intercept value is almost negligible(when the cost function value is close to minima).
![4) b vs epochs](https://user-images.githubusercontent.com/37456341/158860330-b6a53045-e61a-454c-9189-2936f9f3ffd1.gif)

## Slope(m) V/S epochs plot

* Intially the slope value is increasing with iterations.
* After some iterations the change in slope is almost negligible(when the cost function value is close to minima).

![5) m vs epochs](https://user-images.githubusercontent.com/37456341/158860269-978b3988-bf44-4960-904f-5b283c130c8d.gif)

## Contour plot

Contour plots (sometimes called Level Plots) are a way to show a three-dimensional surface on a two-dimensional plane.

![6) contour plot](https://user-images.githubusercontent.com/37456341/158860386-c51c9f0f-30f6-4724-b8f2-cc2caaef974c.gif)

## Effect of learning rate on Gradient Descent Algorithm

Gradident Descent algorithm is very sensitive to the learning rate.

### Following are the three possible effects:
#### 1) Best learning rate

Here the algorithm converge within the defined epochs/iterations.
![7) best learning rate](https://user-images.githubusercontent.com/37456341/158860410-b9049548-de84-4eff-a961-1d8a4f32ed58.gif)



#### 2) Low learning rate

Here the steps are going to be very small, hence the algorithm might not converge within the defined epochs.
![8) low learning rate](https://user-images.githubusercontent.com/37456341/158860454-6322b1e7-83e6-40f6-a87f-aae7cea7ce37.gif)

#### 3) High learning rate

Here the steps are going to be large, hence the algorithm will never converge to the minima.
![9) high learning rate](https://user-images.githubusercontent.com/37456341/158859758-82f9f9e4-ed02-4e7b-906d-53ff9bd939d4.gif)



## Gradient Descent algorithm Visualisation
![3) cost function](https://user-images.githubusercontent.com/37456341/158860221-5ad2743a-cc6b-4370-a92a-955d97e39f83.gif)

* step 3: After getting the best fit line we can predict the desired outcomes.

