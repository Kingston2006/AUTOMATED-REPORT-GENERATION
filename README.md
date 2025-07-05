COMPANY: CODTECH IT SOLUTIONS

"NAME: KINGSTON

"INTERN ID: CTO4DG46

"DOMAIN: PYTHON PROGRAMMING

DURATION: 4 WEEEKS

MENTOR: NEELA SANTOSH


Automated Data Analysis Report Generator in Google Colab
This Python-based tool offers a streamlined solution for quick, automated exploratory data analysis (EDA) using Google Colab. It allows users to upload a CSV file, generate summary statistics and a correlation heatmap, and export all insights into a well-formatted PDF report. It’s an ideal tool for analysts, data scientists, educators, or students who want fast, sharable insights from tabular data without manual formatting.

Key Libraries Used
pandas: For data manipulation and generating summary statistics.

seaborn & matplotlib: For creating the correlation heatmap visualization.

fpdf2: To generate multi-page PDF reports with structured content and embedded images.

Google Colab’s files module: For uploading CSV files and downloading the final report.

Step-by-Step Workflow
Library Installation and Setup
The script begins by installing all necessary packages using pip, ensuring compatibility in the Colab environment. This includes libraries for data analysis (pandas, seaborn, matplotlib) and PDF generation (fpdf2).

File Upload
Users are prompted to upload a .csv file via Google Colab’s file picker. The uploaded filename is automatically extracted, and the data is read into a pandas DataFrame.

Descriptive Statistics
The script computes key statistical summaries (count, mean, std, min, quartiles, and max) for all numerical columns using df.describe(), rounded to two decimal places for clarity. This summary is later formatted into a table within the PDF report.

Correlation Heatmap
A correlation matrix is calculated using df.corr(numeric_only=True), and visualized as a heatmap using Seaborn. The figure includes a title and uses the "coolwarm" color palette for better interpretability. The heatmap is saved as an image file (correlation_heatmap.png) for inclusion in the PDF.

PDF Report Generation
A multi-page PDF is created using FPDF, with the following structure:

Page 1 – Cover Page
Displays the title of the report, dataset name, and shape (number of rows and columns).

Page 2 – Descriptive Statistics
Presents the describe() table as a grid, including all metrics and columns. The layout dynamically adjusts based on the number of columns in the dataset.

Page 3 – Correlation Heatmap
Embeds the heatmap image to visually present relationships between numerical variables.

Exporting the PDF
The report is saved as data_analysis_report.pdf and automatically offered for download using files.download(). This final step allows users to easily share or archive the results of their quick EDA.

Advantages and Use Cases
No local setup required: Runs entirely in Google Colab.

Fast and automatic: Generates a formatted report in seconds with minimal code changes.

Portable insights: Produces a professional-looking PDF for presentations, documentation, or sharing.

Educational use: Helps beginners understand data analysis pipelines.


![Image](https://github.com/user-attachments/assets/26f5ddc0-6f52-48d8-bfb6-b7aed9e31442)
![Image](https://github.com/user-attachments/assets/6bdd5e2c-4ef4-4b21-a695-d8310623b8dc)
