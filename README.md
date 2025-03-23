# Green-Taxi-Data-Analytics-Predictive-and-Optimization-Model

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<h1>TP Project Phase I</h1>
<h2>Description</h2>
<p>This project is part of the "Transportation Planning" course at Sharif University of Technology, under the supervision of Dr. Hassan Naeibi. The objective of Phase I is to preprocess, analyze, and interpret a dataset containing records of rides provided by Green Taxi services in New York City. The dataset includes information such as pickup and drop-off locations, trip distances, fares, and additional charges. The project also involves applying machine learning techniques to predict trip costs and categorize payment methods.</p>
<h2>Project Objectives</h2>
<ol>
<li><strong>Data Preprocessing:</strong>
<ul>
<li>Remove irrelevant columns.</li>
<li>Handle missing data for specific fields (e.g., filling missing tips for trips paid by credit card).</li>
<li>Clean data where passenger count exceeds four for van dispatch trips or has unknown trip/payment types.</li>
<li>Remove rows with empty <code>VendorID</code> or data from years other than 2021.</li>
</ul>
</li>
<li><strong>Data Analysis:</strong>
<ul>
<li>Generate heat maps to visualize peak hours and analyze daily trends.</li>
<li>Analyze trip types, passenger payment patterns, and borough-specific dynamics.</li>
<li>Provide insights into usage trends with relevant graphs.</li>
</ul>
</li>
<li><strong>Advanced Analysis and Modeling:</strong>
<ul>
<li>Perform correlation analysis and build regression models for trip cost prediction using techniques like backward selection, chi-square tests, and random forest importance.</li>
<li>Create classification models to predict whether tips were paid using algorithms such as Decision Tree, XGBoost, and Random Forest.</li>
<li>Optimize models using methods like Taguchi or Grid Search, ensuring efficient hyperparameter tuning.</li>
</ul>
</li>
<li><strong>Creative Modeling:</strong>
<ul>
<li>Develop innovative solutions combining multiple methods and provide references to relevant research papers for implementation.</li>
</ul>
</li>
</ol>
<h2>Dataset Overview</h2>
<p>The dataset includes the following key fields:</p>
<ul>
<li><code>VendorID</code>: Identifier for the TSP responsible for the trip record.</li>
<li><code>datetime_pickup_lpep</code>: Time and date of trip start.</li>
<li><code>datetime_dropoff_lpep</code>: Time and date of trip end.</li>
<li><code>PULocationID</code> and <code>DOLocationID</code>: Pickup and drop-off locations.</li>
<li><code>count_passenger</code>: Number of passengers.</li>
<li><code>distance_trip</code>: Trip distance in miles.</li>
<li><code>amount_fare</code>: Fare amount excluding tips and taxes.</li>
<li><code>amount_tip</code>: Tip amount paid via credit card.</li>
<li><code>amount_tolls</code>: Toll charges during the trip.</li>
<li><code>type_payment</code>: Payment method (e.g., cash, credit card).</li>
<li><code>type_trip</code>: Trip type (e.g., airport, local).</li>
<li>Additional fields like <code>surcharge_congestion</code>, <code>tax_mta</code>, and <code>extra</code> for various charges.</li>
</ul>
</body>
</html>
