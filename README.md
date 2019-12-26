# linear_regression

Our original model for exponential growth is:

C=A0rt 

Where  C  is transistor the count and  t  is the year.

r  is the rate of growth. For example, when  t  goes from 1 to 2,  C  increases by a factor of  r . When  t  goes from 2 to 3,  C  increases by a factor of  r  again.

When we take the log of both sides, we get:

logC=logr∗t+logA0 

This is our linear equation:

y^=ax+b 

Where:

y^=logC 
a=logr 
x=t 
b=logA0 

We are interested in  r , because that's the rate of growth. Given our regression weights, we know that:

a=0.34188038 

so that:

r=e0.34188038=1.4076 

To find the time it takes for transistor count to double, we simply need to find the amount of time it takes for  C  to increase to  2C .

Let's call the original starting time  t , to correspond with the initial transistor count  C .

Let's call the end time  t′ , to correspond with the final transistor count  2C .

Then we also have:

2C=A0rt′ 

Combine this with our original equation:

C=A0rt 

We get (by dividing the 2 equations):

2C/C=(A0rt′)/A0rt 

Which simplifies to:

2=r(t′−t) 

Solve for  t′−t :

t′−t=log2logr=log2a 

Important note! We haven't specified what the starting time  t  actually is, and we don't have to since we just proved that this holds for any  t .
