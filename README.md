<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Green Taxi Data Analytics: Predictive and Optimization Model</title>
</head>
<body>
<h1>Green Taxi Data Analytics: Predictive and Optimization Model</h1>

<!-- Phase I -->
<h2>TP Project Phase I</h2>
<h3>Description</h3>
<p>This project is part of the "Transportation Planning" course at Sharif University of Technology, under the supervision of Dr. Hassan Naeibi. The objective of Phase I is to preprocess, analyze, and interpret a dataset containing records of rides provided by Green Taxi services in New York City. The dataset includes information such as pickup and drop-off locations, trip distances, fares, and additional charges. The project also involves applying machine learning techniques to predict trip costs and categorize payment methods.</p>

<h3>Project Objectives</h3>
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

<h3>Dataset Overview</h3>
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

<!-- Phase II -->
<h2>TP Project Phase II</h2>
<h3>Description</h3>
<p>Phase II builds upon the insights from Phase I and aims to provide actionable recommendations and advanced solutions for optimizing transportation planning and operations. The focus is on OD matrix extraction, revenue optimization, demand prediction, and supply-demand adjustment methods for Green Taxi services in New York City.</p>

<h3>Project Objectives</h3>
<ol>
<li><strong>OD Matrix Analysis:</strong>
<ul>
<li>Extract OD matrices for all boroughs in the city.</li>
<li>Identify borough pairs with the highest percentage of trips between them.</li>
<li>Determine the borough with the highest percentage of internal trips (same origin and destination).</li>
<li>Assume you are a new supplier entering this market. Based on insights gained from this analysis, what decisions would you take?</li>
</ul>
</li>
<li><strong>Revenue Optimization:</strong>
<ul>
<li>A Chinese supplier plans to enter NYC’s Green Taxi market next year. They aim to maximize revenue while operating within constraints, such as a fixed daily budget of $40 per vehicle and a maximum service distance of 1,000 kilometers per day.</li>
<li>Define the optimization problem for maximizing revenue while considering operational constraints such as charging infrastructure and limited activity days.</li>
<li>Provide recommendations for vehicle operations based on your analysis.</li>
</ul>
</li>
<li><strong>Time-Based Route Grouping:</strong>
<ul>
<li>Group daily routes into time-based groups (low traffic, normal traffic, heavy traffic).</li>
<li>Extract a 25×25 OD submatrix representing daily average demand between all zones.</li>
<li>Identify the OD pairs with the highest weights (most demand). Construct this submatrix.</li>
<li>Balance supply and demand using one of the adjustment methods, incorporating dummy zones if necessary.</li>
</ul>
</li>
<li><strong>Demand Prediction:</strong>
<ul>
<li>Use a gravity model with resistance functions (e.g., exponential and log-normal) to predict future demand for the next year. Assume β = 0.1 and β = 0.3.</li>
<li>Evaluate the accuracy of the models using RMSE and R-squared metrics.</li>
<li>Choose the best model and justify your selection with reasoning based on the evaluation metrics.</li>
</ul>
</li>
<li><strong>Cost Matrices:</strong>
<ul>
<li>Estimate the average cost for each route (round trip) within each time group.</li>
<li>Create a cost matrix based on the average round-trip price for each time group.</li>
<li>Estimate the average distance between any two zones and construct a distance matrix.</li>
</ul>
</li>
<li><strong>Tip Prediction:</strong>
<ul>
<li>Incorporate tips into the objective function for revenue optimization. Predict the likelihood of tip payments using probabilistic models.</li>
<li>Use the Phase I prediction model to forecast tip payments and assess its accuracy.</li>
<li>Include dimensions such as time groups, origin, destination, and trip costs in the decision variables.</li>
<li>Analyze the likelihood of tip payments with a fixed probability (e.g., $5 tips) and incorporate this into the optimization process.</li>
</ul>
</li>
</ol>

<h3>Additional Information</h3>
<p>Assumptions:</p>
<ul>
<li>All vehicles have a constant speed.</li>
<li>Charging infrastructure and operational limits are considered.</li>
</ul>
<p>Deliverables for Phase II include Python code files and a report file. Files should be named as follows: <code>TP Project Phase II student_number_1, student_number_2, student_number_3</code>.</p>
</body>
</html>
