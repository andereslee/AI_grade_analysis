# Intelligent Grade Q&A Program

This project implements an intelligent question and answer program that focuses on analyzing student grades and generating responses based on user queries. The program supports text answers, table display, as well as the generation of bar charts, line charts, and scatter plots.

### Usage Instructions

1. **Text Answer Format**:
   - Based on user queries, return answers in the following format:
     ```
     {"answer": "<Your answer goes here>"}
     ```
     For example:
     ```
     {"answer": "The product ID with the highest order quantity is 'MNWC3-067'"}
     ```

2. **Table Format**:
   - If users require a table, return the data in the following format:
     ```
     {"table": {"columns": ["column1", "column2", ...], "data": [[value1, value2, ...], [value1, value2, ...], ...]}}
     ```

3. **Bar Chart, Line Chart, and Scatter Plot Format**:
   - If users request a specific type of chart, respond in the corresponding format:
     - Bar Chart:
       ```
       {"bar": {"columns": ["A", "B", "C", ...], "data": [34, 21, 91, ...]}}
       ```
     - Line Chart:
       ```
       {"line": {"columns": ["A", "B", "C", ...], "data": [34, 21, 91, ...]}}
       ```
     - Scatter Plot:
       ```
       {"scatter": {"columns": ["A", "B", "C", ...], "data": [34, 21, 91, ...]}}
       ```
   Note: The program only supports these three types of charts: "bar", "line", and "scatter".

4. **Max Progress Student Response**:
    - If users inquire about "The student with the maximum progress between exam n and exam n-1 in each class," generate the response based on the provided logic.

### Code Example

```python
# Code snippet
import json
from langchain_openai import ChatOpenAI
from langchain_experimental.agents.agent_toolkits import create_pandas_dataframe_agent
...
# More code content can be found in the provided code sample above

# Return all outputs as JSON strings. Ensure column names and data values are surrounded by double quotes.

# Example user query processing 
```

### User Guide

- Upload a CSV file for AI assistance in grade analysis and data visualization.
- Choose different tool functions, including one-click grade summary, manual grade visualization, and AI grade analysis.
- Input your questions or requests and click "Generate Answer" to query.
- Based on the response type, the program will display the results in text, table, or chart format.

### Program Creator

🐯

Thank you for using the Intelligent Grade Q&A Program! If you need any assistance or have any questions, feel free to contact us.
