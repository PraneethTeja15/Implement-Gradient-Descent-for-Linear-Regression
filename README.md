# Implement-Gradient-Descent-for-Linear-Regression
To implement linear regression using Gradient Descent from scratch (without using scikit-learn’s LinearRegression). Your task is to compare the closed-form solution (Normal Equation) with Gradient Descent on the same dataset.
🚀 Linear Regression: Normal Equation vs Gradient Descent
👨‍🎓 Student Info
Name: Jilkapally Praneeth Teja

Student ID: [Your ID here]

Assignment: Implement Linear Regression using both the Normal Equation and Gradient Descent (without using scikit-learn’s LinearRegression)

📖 Problem Statement
The objective of this assignment is to build Linear Regression from scratch using two approaches:

Closed-Form (Normal Equation)

Iterative (Gradient Descent)

Both models are trained on the same dataset to compare their parameter estimates, predictions, and performance.

📊 Dataset
Generated 200 samples with:

𝑦
=
3
+
4
𝑥
+
𝜖
where 
𝜖
∼
𝑁
(
0
,
1
)
y=3+4x+ϵwhere ϵ∼N(0,1)
𝑥
∈
[
0
,
5
]
x∈[0,5], uniformly spaced.

Added Gaussian noise to simulate real-world data.

🛠️ Implementation
1️⃣ Dataset Generation

Created 200 samples for 
𝑥
x.

Added Gaussian noise.

Plotted the raw data points.

2️⃣ Closed-Form Solution (Normal Equation)

Added a bias column of 1’s to 
𝑋
X.

Computed parameters using:

𝜃 =(𝑋𝑇
𝑋
)
−
1
𝑋
𝑇
𝑦
θ=(X 
T
 X) 
−1
 X 
T
 y
Printed intercept and slope.

Plotted the fitted line over the data.

3️⃣ Gradient Descent

Initialized 
𝜃
=
[
0
,
0
]
θ=[0,0].

Learning rate: 
𝜂
=
0.05
η=0.05.

Iterations: 1000.

Tracked and plotted loss (MSE vs iterations).

Printed final intercept and slope.

4️⃣ Comparison

Reported parameters from both approaches.

Verified that Gradient Descent converged to the same solution as the Normal Equation.

📈 Results
Method	Intercept	Slope
Closed-Form	~3.01	~3.99
Gradient Descent	~3.01	~3.99

✅ Both methods produced nearly identical results.

📝 Short Explanation
Both the Normal Equation and Gradient Descent minimized the same convex Mean Squared Error cost function, which is why they converged to almost the same parameters. The Normal Equation provides the exact solution in one step, while Gradient Descent iteratively approaches the same values — confirmed by the decreasing loss curve.
