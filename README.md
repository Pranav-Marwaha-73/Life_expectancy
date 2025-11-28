<h1>📈 Life Expectancy Prediction using Advanced Regression Models</h1>
<h3>🏷️ Machine Learning • Regression • XGBoost • Data Science</h3>

<hr/>

<h2>📝 Abstract</h2>
<p>
This project presents a machine-learning-driven approach to accurately <strong>predict life expectancy</strong> using a comprehensive 
<strong>15-year dataset across 193 countries</strong> from Kaggle. 
The workflow includes two-stage EDA, kNN imputation, categorical encoding, benchmarking 40+ regression models via LazyPredict, 
and hyperparameter tuning. 
The <strong>XGBRegressor</strong> emerged as the best-performing model with an exceptional <strong>R² score of 96.87%</strong>.
</p>

<hr/>

<h2>🎯 Key Objectives</h2>
<ul>
  <li>📊 Conduct detailed Exploratory Data Analysis (EDA)</li>
  <li>🔍 Implement kNN imputation for missing values</li>
  <li>⚡ Benchmark 40+ regression models using LazyPredict</li>
  <li>🔧 Perform Hyperparameter Tuning for top models</li>
  <li>🤖 Build an accurate XGBRegressor model for life expectancy prediction</li>
</ul>

<hr/>

<h2>📊 Dataset Overview</h2>

<p><strong>Records:</strong> 2,938<br/>
<strong>Features:</strong> 22<br/>
<strong>Countries:</strong> 193<br/>
<strong>Years Covered:</strong> 15<br/>
<strong>Target Variable:</strong> Life expectancy</p>

<h3>🔎 Feature Categories</h3>

<table>
  <thead>
    <tr>
      <th>Category</th>
      <th>Features</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Demographic</strong></td>
      <td>Country, Year, Status</td>
    </tr>
    <tr>
      <td><strong>Health Factors</strong></td>
      <td>Life expectancy, Adult mortality, Infant deaths, Under-five deaths, Hepatitis B, Measles, Polio, Diphtheria, HIV/AIDS, BMI, Thinness indicators</td>
    </tr>
    <tr>
      <td><strong>Economic Factors</strong></td>
      <td>GDP, Schooling, Income composition of resources, Percentage expenditure, Total expenditure</td>
    </tr>
    <tr>
      <td><strong>Population</strong></td>
      <td>Population</td>
    </tr>
    <tr>
      <td><strong>Categorical</strong></td>
      <td>Country (193 unique), Status (Developed/Developing)</td>
    </tr>
  </tbody>
</table>

<hr/>

<h2>🛠️ Methodology and Pipeline</h2>

<h3>1️⃣ Data Preprocessing</h3>
<ul>
  <li>🧼 Data cleaning and formatting</li>
  <li>🩹 Missing value handling (Mean + kNN Imputation)</li>
  <li>🔠 Label Encoding for categorical values</li>
</ul>

<h3>2️⃣ Model Benchmarking</h3>
<p>Used <strong>LazyPredict</strong> to rapidly train and evaluate over <strong>40 regression models</strong>.</p>

<h3>3️⃣ Hyperparameter Tuning</h3>
<p>Top-performing models were optimized using Grid Search / Random Search with Cross Validation.</p>

<h3>4️⃣ Final Model Selection</h3>
<p>The optimized models were evaluated on a held-out test set. The best-performing model was selected.</p>

<hr/>

<h2>✅ Results & Conclusion</h2>

<table>
  <thead>
    <tr>
      <th>Model</th>
      <th>Metric</th>
      <th>Score</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>XGBRegressor (Optimized)</strong></td>
      <td>R² Score</td>
      <td><strong>96.87%</strong></td>
    </tr>
    <tr>
      <td><strong>XGBRegressor (Optimized)</strong></td>
      <td>RMSE</td>
      <td>Very Low</td>
    </tr>
  </tbody>
</table>

<p>
The model explains <strong>~97% of the variance</strong> in life expectancy, highlighting the strength of ensemble learning 
and the value of robust preprocessing.
</p>

<hr/>

<h2>📁 Project Structure</h2>

<pre>
📦 Life-Expectancy-Prediction
├── 📄 README.md
├── 📓 notebooks/
│   └── EDA_and_Model.ipynb
├── 🗂️ data/
│   └── life_expectancy.csv
├── 🧠 models/
│   └── xgb_regressor.pkl
└── 🧪 src/
    ├── preprocessing.py
    ├── model_training.py
    └── evaluation.py
</pre>

<hr/>

<h2>📚 References</h2>
<ul>
  <li><strong>XGBoost:</strong> Chen, T., & Guestrin, C. (2016). "XGBoost: A Scalable Tree Boosting System."</li>
  <li><strong>kNN Imputation:</strong> Troyanskaya, O., et al. (2001). "Missing value estimation methods for DNA microarray data."</li>
</ul>

<hr/>

<h2>⭐ Like this project?</h2>
<p>If you found this project useful, please ⭐ star the repository!</p>
