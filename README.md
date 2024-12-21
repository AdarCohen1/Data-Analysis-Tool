# Data-Analysis-Tool

This project is an interactive data analysis tool implemented in Python for analyzing user activities, document usage, and operational trends. It is designed with a graphical interface for ease of use and features detailed visualizations and customizable analysis.

Key Functionalities
1. Data Handling
JSON Upload: Users can upload local JSON files containing activity logs for analysis.
Cloud Integration: The tool retrieves activity data from a Firebase cloud database for dynamic analysis.
2. User Interface
Interactive Widgets:
Radio buttons for data selection (local file vs. cloud).
Drop-downs and buttons to select specific analysis functions.
Chat-like interface for keyword-based navigation.
Keyword Matching:
Uses fuzzywuzzy to detect user input and map it to relevant analysis functions based on keywords.
3. Analysis Modules
The tool provides multiple modules for analyzing and visualizing data:

Tab Time Analysis: Calculate and display the average time users spend on specific tabs or documents.
Activity Timeline: Visualize the timeline of document opening and closing events for each user.
Frequent Actions: Identify the most frequent actions and show the number of actions performed by each user.
Document Time Analysis: Determine the total working time spent on individual documents by users.
Operations Distribution: Analyze the distribution of various operations across documents and users.
Daily Activity Trends: Display the amount of user activity over time with line graphs.
Glossary Index Comparison: Compare activity logs with an indexed glossary of terms fetched from the Onshape glossary page.
Document Usage Distribution: Visualize which documents are accessed most frequently by users.
4. Text Preprocessing
Stop Words Removal: Filters out common stop words to focus on meaningful terms.
Stemming: Uses PorterStemmer to reduce words to their base forms for efficient indexing.
Word Count: Tokenizes and counts word occurrences in the activity data for further analysis.
5. Web Scraping
Fetches a glossary of terms from Onshape’s help page using BeautifulSoup.
Compares glossary terms with processed JSON data to identify term frequency matches.
6. Visualization
Generates a variety of charts using matplotlib:
Bar charts for document time distribution.
Line plots for user activity trends over time.
Stacked bar charts for document usage by user.
How It Works
Run the Notebook:

Start the notebook in Google Colab or a Jupyter environment.
Install any missing dependencies.
Choose Data Source:

Upload a JSON file or fetch data directly from the Firebase cloud.
Select Analysis:

Use buttons, dropdowns, or text input to trigger specific analysis functions.
View Results:

Graphs and tables are dynamically generated and displayed based on user selections.
Keyword Search:

Enter descriptive phrases (e.g., "average time per tab") in the chat interface to quickly access relevant analysis functions.
Installation
Prerequisites
Python 3.7 or higher
Required libraries:
pandas,
matplotlib,
ipywidgets,
firebase,
fuzzywuzzy,
BeautifulSoup.

Adding some screenshots of the GUI:

Home page:
![image](https://github.com/user-attachments/assets/e8526dad-1af1-4570-9e72-2d5132a5d714)

Choosing the most active action that student used:
![image](https://github.com/user-attachments/assets/d71c4008-a47a-47fe-9aa1-8299e0014293)


User work time on the project (based on infromation from the JSON file):
![image](https://github.com/user-attachments/assets/a9933471-4bc9-415e-a0e3-d3cdac43f7fe)


Count the activity actions of one or more students (on the image I chose all students):
![image](https://github.com/user-attachments/assets/426670fe-5219-48a0-bad2-2301a1b3cbda)



