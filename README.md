<img width="744" height="424" alt="Screenshot 2026-05-05 at 12 35 47 AM" src="https://github.com/user-attachments/assets/181f83f9-8fd6-4351-b763-c50417b42aa0" />

📌 Project Overview: \
•Built a real-time healthcare data pipeline on GCP to process streaming patient vitals and generate risk insights.\
•Implements Medallion Architecture (Bronze, Silver, Gold) for structured data processing.\
•Enables near real-time patient monitoring and analytics using cloud-native tools.\

⚙️ Tech Stack: \
•Google Cloud Pub/Sub – real-time data ingestion\
•Apache Beam (Dataflow) – stream processing\
•Google Cloud Storage (GCS) – Bronze & Silver layers\
•BigQuery – Gold layer analytics\
•Python – pipeline + simulator\
•Looker Studio (optional) – dashboard visualization\

🏗️ Architecture: \
•Bronze Layer: Raw streaming data stored in GCS\
•Silver Layer: Cleaned + validated + enriched data\
•Gold Layer: Aggregated patient-level insights in BigQuery\

🚀 Key Features: \
•Processes 50–100 events/sec with <60s latency\
•Handles real-time streaming ingestion\
•Filters invalid records (~10% error rate simulation)\
•Computes patient risk score & risk levels (Low/Moderate/High)\
•Performs windowed aggregation (1-minute windows)\
•Stores analytics-ready data in BigQuery\

🔄 Data Pipeline Flow: \
•Simulator generates patient vitals\
•Publishes data to Pub/Sub\
•Dataflow pipeline processes stream\
•Writes:\
•Raw → GCS (Bronze)\
•Cleaned → GCS (Silver)\
•Aggregated → BigQuery (Gold)\
•Data Studio Report\
