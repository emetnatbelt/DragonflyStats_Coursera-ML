Logistic Regression

5 questions
%===================================================%
1. 
Suppose that you have trained a logistic regression classifier, and it outputs on a new example x a prediction hθ(x) = 0.2. This means (check all that apply):

**Our estimate for P(y=0|x;θ) is 0.8. (correcta)**

**Our estimate for P(y=1|x;θ) is 0.2.  (correcta)**

Our estimate for P(y=0|x;θ) is 0.6.

Our estimate for P(y=1|x;θ) is 0.4.
1
%===================================================%
2. 
Suppose you have the following training set, and fit a logistic regression classifier hθ(x)=g(θ0+θ1x1+θ2x2).

Which of the following are true? Check all that apply.

1. **J(θ) will be a convex function, so gradient descent should converge to the global minimum. (CORRECTA)**

2. **Adding polynomial features (e.g., instead using h_{θ}(x)=g(θ0+θ1x1+θ2x2+θ3x21+θ4x1x2+θ5x22) ) could increase how well we can fit the training data.(CORRECTA)**

3. The positive and negative examples cannot be separated using a straight line. So, gradient descent will fail to converge.

4. Because the positive and negative examples cannot be separated using a straight line, linear regression will perform as well as logistic regression on this data.

%===================================================%
3. 
For logistic regression, the gradient is given by ∂∂θjJ(θ)=1m∑mi=1(hθ(x(i))−y(i))x(i)j. Which of these is a correct gradient descent update for logistic regression with a learning rate of α? Check all that apply.



a) θ:=θ−α1m∑mi=1(θTx−y(i))x(i).


b) __** θj:=θj−α1m∑mi=1(hθ(x(i))−y(i))x(i)j (simultaneously update for all j).**__
 
c) θj:=θj−α1m∑mi=1(hθ(x(i))−y(i))x(i) (simultaneously update for all j).

d) __**CORRECT θj:=θj−α1m∑mi=1(11+e−θTx(i)−y(i))x(i)j (simultaneously update for all j).**__

%===================================================%

4. 
Which of the following statements are true? Check all that apply.

_** The sigmoid function g(z)=11+e−z is never greater than one (>1).

_** The cost function J(θ) for logistic regression trained with m≥1 examples is always greater than or equal to zero.

For logistic regression, sometimes gradient descent will converge to a local minimum (and fail to find the global minimum). This is the reason we prefer more advanced optimization algorithms such as fminunc (conjugate gradient/BFGS/L-BFGS/etc).

WRONG Linear regression always works well for classification if you classify by using a threshold on the prediction made by linear regression.

%-----------------------%

_** The one-vs-all technique allows you to use logistic regression for problems in which each y(i) comes from a fixed, discrete set of values.

For logistic regression, sometimes gradient descent will converge to a local minimum (and fail to find the global minimum). This is the reason we prefer more advanced optimization algorithms such as fminunc (conjugate gradient/BFGS/L-BFGS/etc).

_** The cost function J(θ) for logistic regression trained with m≥1 examples is always greater than or equal to zero.

Since we train one classifier when there are two classes, we train two classifiers when there are three classes (and we do one-vs-all classification).

%===================================================%

5. 
Suppose you train a logistic classifier hθ(x)=g(θ0+θ1x1+θ2x2). Suppose θ0=−6,θ1=0,θ2=1. Which of the following figures represents the decision boundary found by your classifier?

WRONG % 1 | 0 vertical
Figure:



** Y=0 | Y=1 vertical (X1 >=6)**

Figure:


% 0 | 1 horizontal

Figure:


% 1 | 0 horizontal

Figure:


%===================================================%

