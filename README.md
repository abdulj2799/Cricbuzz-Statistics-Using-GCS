# Cricbuzz-Statistics-Using-GCS

In data engineering, converting raw data into meaningful visualizations involves overcoming various challenges and celebrating successes. This guide explores the process of building a cricket statistics pipeline using Google Cloud services, from retrieving data via the Cricbuzz API to developing an interactive Looker Studio dashboard, enabling seamless data analysis and visualization.

#### Architecture
![image](https://github.com/user-attachments/assets/5bf4f299-bffc-48a1-8b5e-bd904b662be0)

#### Integrating Python with the Cricbuzz API for Data Collection  
Our journey begins with Python's ability to interact with APIs. We'll explore how to retrieve cricket statistics from the Cricbuzz API, leveraging Python to efficiently extract and process the required data.  

#### Storing Data Securely in Google Cloud Storage (GCS)  
Once collected, the data must be securely stored in the cloud. We'll discuss how to save it in CSV format within Google Cloud Storage (GCS), ensuring both accessibility and scalability for future processing.  

#### Configuring a Cloud Function Trigger  
After storing the data, the next step is setting up a Cloud Function that automatically triggers upon a new file upload in our GCS bucket. This serves as the entry point for subsequent data processing stages.  

#### Executing the Cloud Function  
The Cloud Function is programmed to seamlessly initiate a Dataflow job. We will focus on configuring triggers and passing the necessary parameters to ensure a smooth and automated data processing workflow.  

#### Running a Dataflow Job for BigQuery Integration  
A key component of our pipeline is the Dataflow job, triggered by the Cloud Function. This job transfers data from the CSV file in GCS to BigQuery. We will optimize the job settings to enhance performance and ensure accurate data migration.  

#### Building a Looker Studio Dashboard  
Finally, we will connect BigQuery as a data source to Looker Studio, enabling the creation of an interactive dashboard. This dashboard will serve as a central hub for visualizing and analyzing cricket statistics, providing valuable insights.

![image](https://github.com/user-attachments/assets/fcc509af-33d8-405b-8101-09eed5c258f8)
