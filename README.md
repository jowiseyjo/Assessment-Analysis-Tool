Assessment Analysis Tool
Overview
The Assessment Analysis Tool is a Python-based desktop application designed to help educators, researchers, and assessment practitioners perform automatic analysis of test items.
The software provides tools for:
Generating simulated student response data
Uploading real assessment datasets
Performing automatic item analysis
Estimating test reliability using Cronbach's Alpha
Producing graphical visualizations of assessment results
Generating professional PDF item analysis reports
The system uses a simple Graphical User Interface (GUI) to make statistical analysis accessible even to users without programming knowledge.
Key Features
1.	Simulated Data Generator
Users can generate simulated binary test response data by specifying:
Number of pupils
Number of test items
The simulator uses a probabilistic logistic model to generate realistic response patterns.
Outputs generated:
CSV dataset of simulated responses
Full PDF item analysis report
2.	Upload Real Test Data
Users can upload their own CSV dataset containing student responses.
Requirements:
Rows represent students
Columns represent test items
Responses should be coded as 0 (incorrect) or 1 (correct)
The software will automatically analyze the uploaded data and produce a PDF report.
3.	Automatic Item Analysis
For each test item, the software calculates:
Item Difficulty (p-value)
Item Discrimination (item-total correlation)
Item Recommendation
Items are automatically classified as:
Good Item
Too Easy
Too Difficult
Review Item
4.	Test Reliability Estimation
The software computes Cronbach's Alpha, a widely used measure of test reliability in educational measurement.
This helps determine whether a test is internally consistent and suitable for assessment purposes.
5.	Graphical Analysis
The generated report includes graphical summaries such as:
Distribution of total test scores
Item difficulty distribution
Item Characteristic Curves (ICCs)
These visualizations help users better interpret the quality of their assessment items.
6.	Automatic PDF Report Generation
The system automatically generates a professional item analysis report in PDF format.
The report includes:
Test summary information
Item analysis table
Reliability estimate
Graphical visualizations
Interpretation guidelines
Example Outputs
The software generates:
simulated_data.csv
simulated_data_report.pdf
uploaded_data_report.pdf
Technology Stack
This project is implemented using the following technologies:
Python
Tkinter – Graphical User Interface
NumPy – Numerical computing
Pandas – Data analysis
Matplotlib – Graph generation
ReportLab – PDF report creation
Installation
Step 1: Install Python
Download and install Python from:
https://www.python.org
Python 3.8 or later is recommended.
Step 2: Install Required Libraries
Run the following command:
pip install numpy pandas matplotlib reportlab
Step 3: Run the Application
Run the program using:
python assessment_tool.py
The graphical interface will open automatically.
How to Use the Software
Generate Simulated Data
Enter the number of pupils
Enter the number of test items
Click Generate Simulated Data + PDF
The program will generate:
A simulated dataset
A PDF item analysis report
Analyze Real Data
Click Upload Real Data CSV for PDF Analysis
Select your CSV file
The program will automatically analyze the data and generate a report
Expected CSV Format
Example dataset:
Item_1	Item_2	Item_3	Item_4
1	0	1	1
0	1	1	0
1	1	0	1
Where:
1 = Correct response
0 = Incorrect response
Project Structure
Assessment-Analysis-Tool
│
├── assessment_tool.py
├── README.md
├── requirements.txt
└── .gitignore
Applications
This software can be used for:
Classroom test analysis
Educational assessment research
Measurement and evaluation studies
Learning analytics
Test development and validation
Developer
Johnson E. Iyen
Email: jowisey@gmail.com
Phone: +2347030429845
License
This project is available for educational and research purposes.

