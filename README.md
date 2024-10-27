
# NYPD Traffic Accidents Analysis - Dashboard

### Downloadable PDF Link : https://acrobat.adobe.com/id/urn:aaid:sc:AP:68be3285-8668-40e5-9b64-7c483efaf8ea

## NYC Traffic Accident Analysis

### Data Ingestion:
Imported NYPD motor vehicle collision data (Jan-Aug 2020) using Power Query, including date, time, location (borough, ZIP, street, lat/lon), vehicles, victims, and contributing factors.
### Data Modeling:
Developed star schema with DAX measures and calculated columns to establish relationships and key metrics.
### Visualizations:
#### Line Charts:
Compared monthly accident percentages to identify seasonal patterns.
####  Heatmaps:
Analyzed accident frequency by day of week and hour of day to determine peak times.
#### Bar Charts:
Identified streets with highest accident reports and their percentage of total accidents.
#### Pie Charts:
Highlighted most common contributing factors overall and for fatal accidents.
#### Business Intelligence:
Addressed key business questions to uncover trends, high-risk periods, and factors influencing fatal collisions.

# Dashboard's Executive Summary Snapshot (Power BI Service)



![dashboard_snapo]([https://private-user-images.githubusercontent.com/79145457/380488627-e7a988cf-028c-45a8-a7b6-531a2c8f0c13.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzAwMjcwMTgsIm5iZiI6MTczMDAyNjcxOCwicGF0aCI6Ii83OTE0NTQ1Ny8zODA0ODg2MjctZTdhOTg4Y2YtMDI4Yy00NWE4LWE3YjYtNTMxYTJjOGYwYzEzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMDI3VDEwNTgzOFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWZjNjAxM2NlZmY4YWRjYTg4MzQ0NDcyYjFkMWE3MzA5NWM4YzdmNGYwZTM2Y2I4ODVkOGIwZWEyMTZlNDI1YzgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.xUZFzeQ8HaL7U0V-qFrUj2R-HQS1qeP_PHzYHPk56XI](https://private-user-images.githubusercontent.com/79145457/380488627-e7a988cf-028c-45a8-a7b6-531a2c8f0c13.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzAwMzMwMTksIm5iZiI6MTczMDAzMjcxOSwicGF0aCI6Ii83OTE0NTQ1Ny8zODA0ODg2MjctZTdhOTg4Y2YtMDI4Yy00NWE4LWE3YjYtNTMxYTJjOGYwYzEzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMDI3VDEyMzgzOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWI0YzU2OTMxYzVkMGIyMWQxMjQxZmNjOTYzMjk1ZjJmOTFlZDk1MDcxZjAyZDhmMzhkN2Q5NjFmNDljNmQ3NWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.w9vzwWmwkoqVnnO4JSYPGPSscVNYJUicfH9u4fQeBAg))



 
 # Report's Time Page (Power BI DESKTOP)



 
![Dashboard_upload](https://private-user-images.githubusercontent.com/79145457/380489486-125de368-2f09-4be0-82ef-e7580236c5cc.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzAwMjc4MjQsIm5iZiI6MTczMDAyNzUyNCwicGF0aCI6Ii83OTE0NTQ1Ny8zODA0ODk0ODYtMTI1ZGUzNjgtMmYwOS00YmUwLTgyZWYtZTc1ODAyMzZjNWNjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMDI3VDExMTIwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTM3NWMwZjZiNmU2OGJlODIxOTVlYzA5OGI5YWE0MDViZDYwYmNlMGQzMTI5NjNkOWMxZDI2ZTQ4Njc2YWNlNDEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.bpZrQt_FpHa6NNZp1fyw_qLYxCyepH9nCuUiT3sR7j8)



 # Report's Location Page



 
![Dashboard_upload](https://private-user-images.githubusercontent.com/79145457/380489486-125de368-2f09-4be0-82ef-e7580236c5cc.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzAwMjc4MjQsIm5iZiI6MTczMDAyNzUyNCwicGF0aCI6Ii83OTE0NTQ1Ny8zODA0ODk0ODYtMTI1ZGUzNjgtMmYwOS00YmUwLTgyZWYtZTc1ODAyMzZjNWNjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMDI3VDExMTIwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTM3NWMwZjZiNmU2OGJlODIxOTVlYzA5OGI5YWE0MDViZDYwYmNlMGQzMTI5NjNkOWMxZDI2ZTQ4Njc2YWNlNDEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.bpZrQt_FpHa6NNZp1fyw_qLYxCyepH9nCuUiT3sR7j8)



 # Report's Accident Factors Page



 
![Dashboard_upload](https://private-user-images.githubusercontent.com/79145457/380496085-a8fcadc2-9d64-4a50-85cf-32a7cced725e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzAwMzE5MzIsIm5iZiI6MTczMDAzMTYzMiwicGF0aCI6Ii83OTE0NTQ1Ny8zODA0OTYwODUtYThmY2FkYzItOWQ2NC00YTUwLTg1Y2YtMzJhN2NjZWQ3MjVlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMDI3VDEyMjAzMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWFjY2Y2YWYyZGVhMTIxZDUyMTAzMTUwMTBlNzk5ODYxZWE1ZDVhZmMxYjU0MjFiNmIyOGIwNDUyNjczYTA4NzUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.F6MYgCnA_3FanTtThR6lnsNidKD08ks2lRmcLD1nNF4)



 # Report's DateTime Tooltip

 

 
![Dashboard_upload](https://private-user-images.githubusercontent.com/79145457/380496157-838cd65a-f9a6-4d17-83fc-c262cc2506e0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzAwMzE5ODcsIm5iZiI6MTczMDAzMTY4NywicGF0aCI6Ii83OTE0NTQ1Ny8zODA0OTYxNTctODM4Y2Q2NWEtZjlhNi00ZDE3LTgzZmMtYzI2MmNjMjUwNmUwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEwMjclMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMDI3VDEyMjEyN1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTc5MTg3YjYxZjA3N2NlYmZlNWM1YWIxMmQ1MDVlZGQ4N2E4ZDRlZWU5NTBjN2I4MTEyNjRkMDhjZTA4Zjg5MzMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.lx5RTDbPxY9UgwFtpvRPVQ0lYH1M818A7W4qZitlItM)

# NYPD Traffic Accidents Analysis-Dashboard.md.txt
Displaying # NYPD Traffic Accidents Analysis-Dashboard.md.txt.
