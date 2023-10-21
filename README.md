# Data-Science Hackathon

**Problem statement**: To predict selling price of the house in a given metro city which consists of 5000 localities

Relevant technical literature related to the problem

1) Language used: python3
 
2) tool used: Anaconda – jupyter Notebook – Python R enabled

3) Libraries: scipy , numpy , scikit, pandas, random(Randnteger ,RandFloat, RandCategories)

4) Have Created a Random Data Set by randomly defining columns



**DESIGN**:
Random technique to be applied
By tossing a coin, chose option to enter a feature
If its 0(head): update with randomly available options
If its 1(tail): update with the default choice (REALISTIC APPROACH)

The dataset is of 5000 rows with 11 columns of different attributes
1) Number of localities, indexed on localities number

2) Type of houses  C:5 rooms
	  					     B:7 rooms
                   A:10 rooms

3) Water source ( 1 for available or 0 for not available)

4) Hypothetical pollution index(range of 1 to 10)

5) Built house between (1990-2010)

6) Educational facilities (1 for available or 0 for not available. Within a range of 3 kilometers)

7) Hypothetical crime rate (range of 1 to 10)

8) Percentage of middle class families (on a scale of 100)

9) Roads(good, bad, moderate)

10) Average price per each house in INR(Indian Rupees)  C:500,000		B:1,000,000		A:2,000,000

11) Decision to buy (yes or no)


Have created 2 models for training and testing of data.
In training model, have selected 80% of the 5000 rows
And for testing data 20% of data.


<br/>

A] **TRAINING DATA**

Let the randomly generated, recommended to buy = y’
Pass 80% of rows to training model now, recommended to buy= y
	
If y=y’ => Right_decision
y not equal to y’ => Wrong decision

Efficiency/Precision = Right_decision/80% of 5000 rows
 
B] **TESTING DATA**

Lets pass 20% of remaining rows to Test Model

Let the randomly generated, recommended to buy = y’
Pass 20% of rows to training model now, recommended to buy= Y

If Y=y’ => Right_decision
y not equal to y’ => Wrong decision
efficiency/precision = Right_decision/20% of 5000

LINEAR REGRESSION EQUATION is used to decrease the actual cost of the house by 20% depending on the attributes

If new reduced cost < actual cost => BUY
If new reduced cost > actual cost => do not BUY

<br/>  

**RESULT**: 

Predicted house type and predicted the selling price of house type based on all above-mentioned features and recommended decision to buy i.e., YES or NO

Training data 80% of 5000 rows
Testing data : 20% of remaining rows
