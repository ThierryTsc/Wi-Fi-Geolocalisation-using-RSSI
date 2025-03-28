📂 Dataset
The dataset consists of four RSSI maps (CSV files: RSSI_1.csv, RSSI_2.csv, RSSI_3.csv, RSSI_4.csv), corresponding to four Wi-Fi gateways covering a cartesian grid where signal strength is measured at each meter.

Each sample consists of:

f1, f2, f3, f4 → Signal strength (RSSI) from four access points

x, y → True position (target values)

🛠 Project Objectives
1️⃣ Data Exploration & Visualization

Plot the 4 RSSI maps in a single graph for better visualization.

2️⃣ Handling Missing Data

Propose and apply a method to handle missing RSSI values.

3️⃣ Neural Network Model

Design a dense neural network to predict (x, y) coordinates.

Choose an appropriate loss function for this regression task.

4️⃣ Model Training & Evaluation

Train the model with a train-test split.

Evaluate performance using the R² score.

Plot loss evolution & R² score for both training and test sets.

5️⃣ Error Analysis

Plot a histogram of prediction errors (distance between predicted and actual positions).

6️⃣ Model Improvement

Propose optimizations to enhance prediction accuracy.

🛠 Technologies Used
Python

Pandas & NumPy (data preprocessing)

Matplotlib & Seaborn (data visualization)

Scikit-learn (data handling, R² metric)

TensorFlow/Keras (neural network implementation)

🚀 Neural Network Model
The model is a fully connected neural network (MLP) with:

Input layer: 4 RSSI values as features

Hidden layers: Dense layers with ReLU activation

Output layer: 2 neurons (x, y coordinates)

Loss function: Mean Squared Error (MSE)

Evaluation metric: R² score

📊 Results & Analysis
Model performance: The R² score evaluates how well the model predicts the (x, y) position.

Error histogram: Distribution of distance errors between predicted and actual locations.

Potential Improvements:

Hyperparameter tuning (learning rate, number of layers/neurons)

Adding dropout for regularization

Exploring alternative models (e.g., CNNs, Gaussian Processes)


