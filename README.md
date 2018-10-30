# EEC731-Homework 6

D(St)reams of Anomalies
==================

The real world does not slow down for bad data
1. Set up a data science project structure in a new git repository in your GitHub account
2. Download the benchmark data set from
https://www.kaggle.com/boltzmannbrain/nab or
https://github.com/numenta/NAB/tree/master/data 
3. Load the one of the data set into panda data frames
4. Formulate one or two ideas on how feature engineering would help the data set to establish additional value using exploratory data analysis
5. Build one or more anomaly detection models to determine the anomalies using the other columns as features
6. Document your process and results
7. Commit your notebook, source code, visualizations and other supporting files to the git repository in GitHub


Dataset
=============
The dataset I chose was the NYC Taxi Anomalies - The file was from Kaggle - https://www.kaggle.com/boltzmannbrain/nab/realKnownCause.zip

The csv file is located in- 'nyc_taxi.csv'


About the dataset
==================

->realKnownCause

This is data for which we know the anomaly causes; no hand labeling.

ambient_temperature_system_failure.csv: The ambient temperature in an office setting.
cpu_utilization_asg_misconfiguration.csv: From Amazon Web Services (AWS) monitoring CPU usage – i.e. average CPU usage across a given cluster. When usage is high, AWS spins up a new machine, and uses fewer machines when usage is low.
ec2_request_latency_system_failure.csv: CPU usage data from a server in Amazon's East Coast datacenter. The dataset ends with complete system failure resulting from a documented failure of AWS API servers. There's an interesting story behind this data in the Numenta blog.
machine_temperature_system_failure.csv: Temperature sensor data of an internal component of a large, industrial mahcine. The first anomaly is a planned shutdown of the machine. The second anomaly is difficult to detect and directly led to the third anomaly, a catastrophic failure of the machine.
nyc_taxi.csv: Number of NYC taxi passengers, where the five anomalies occur during the NYC marathon, Thanksgiving, Christmas, New Years day, and a snow storm. The raw data is from the NYC Taxi and Limousine Commission. The data file included here consists of aggregating the total number of taxi passengers into 30 minute buckets.
rogue_agent_key_hold.csv: Timing the key holds for several users of a computer, where the anomalies represent a change in the user.
rogue_agent_key_updown.csv: Timing the key strokes for several users of a computer, where the anomalies represent a change in the user.


--------------------------------------------------------------------------------------------------------------------------

Code for the project
====================
The notebook for this project can be found in the 1.0-EECS731-HW6.ipynb Jupyter notebook. 


Anomaly Detection Models
===================
Used Isolation Forest to detect anomalies in the dataset.
