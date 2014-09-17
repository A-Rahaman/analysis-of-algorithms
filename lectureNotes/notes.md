# CS561 - Analysis of Algorithms - Course notes

I find it a good exercise to type up my lecture notes for the class and add in
any other TODOS or errers in understanding i may have. 


## Weeks 1 and 2

### Random Variables

What is a random variable? 
IF we roll a fair dice, we can call the outcome of that roll $x$ 

What's the probability of that roll?
And how can we help solve these types of problems?

Tool: INdicator random variables - little hackers that help 'indicate' the
ouctome of a random variable. 

\[ I(X=1) 1 if x = 1, 0 if = 0 \]


Let x = outcome of red die
let y = outcome of the blude die

z = x + y 


linearity of expectation 

Given sequence \[ X_1, X_2, X_3 \]

\[ \sum_1^n E(X_i) \]

\[ E(X) = 3.5 = 1/6, 1/5/ 1/4, 1/3, 1/2, 1 \]

Fact - let x&y be two random vars

Then E(x+y) = E(x) + E(y) 


### Birthday Paradox


Awesome little thing that comes up all the time

given the following:

$n = number of people $
$ m = number of days in the year $
X = random var = number of pairs of people with the same birthday

What is $E(x)$? 

If we define an indicator random variable:

\[ X_{i,J} =1 \text{if} i,j, \text{ have the same birthday} \]
\[ X_{i,J} =0  \text{if not} \]

\[ X = \sum_{i,j} X_{i,j} \]
\[ E(X_{i,j}) = 1 * Pr(X_{i,j} = 1) \]
\[ = 1/m \]
\[ E(x) = E(\sum_{i,j} X_{i,j} ) \] * By linearity of expectation
\[ \sum E(X_{i,j}) \]
\[ E(X) = ( n \choose 2 ) * 1/m \]
\[ = n(n+1) / 2m \]
it follows that:
\[ n(n-1) \geq 2m \implies E(X)\geq 1 \]



