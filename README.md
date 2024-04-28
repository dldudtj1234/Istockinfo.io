# Istockinfo.io
Group: Julian and Young
Project Url:
1.      Project Overview: As two individuals who are both interested in the finance field, we believed that creating web applications that offer stock information might be a good idea. We used the yfinance API to create a web tool that searches, condenses, and displays stock information. The site provides intraday trading prices, historical price graphs, eps and other financial metrics, balance sheet, and cash flow.
2.      Usage Guidelines: The user must input a valid stock ticker into the search bar, then click get info. This will bring them to a page with an information summary, and the option to view a stock chart, a balance sheet, and a cash flow table. The pages can be navigated by pressing the various buttons. The user can hover their mouse over the chart to view various data points.If the user input the tickers that are not in the yahoo finance API, it will redirect to the yahoo finance. The public url is not there yet, and we have to use the testing server url: http://127.0.0.1:5000/. 
3.      Dependencies: We used the yfinance api, the official yahoofinance api, to gather data and index it using our python program, which is enabled by flask. Furthermore, to ensure the smooth operations of this application, several external libraries and modules are used. First of all, Flask. Flask ensures us to use python for the web framework and handle web requests. Requests. This is a simple HTTP library built for us to use. Matplotlib, which is a comprehensive library for creating visualization in python. We used this on creating the chart and graphs for the stock. Plotly is to ensure us to make more interactive and quality graphs. This graph with the plotly allows us to have better quality in the chart, where customers or the users can interact more with. Pandas. This allowed us to return the financial data as dataframe objects, specifically used in the balance sheet and cash flow data.  Unfortunately, we didn’t open up the public url for this website. So in order to run the application, you need to type: python app.py. And use the link:  http://127.0.0.1:5000/.  
4. Project Structure: 
We can first start off with our folder named, “Stock”. Inside of the stock, we have several files and folders. The root directory contains all components of our web applications. We can first start off with the app.py. This is the main python script that runs our flask application. This allows us to handle routing, data fetching from the yahoo finance, data formatting and rendering the HTML templates. Next directory is the templates, which consists of the balance_sheet.html, cash_flow.html, Graph.html, income_statement.html, index.html, and result.html. Everything is self explanatory besides the index and result.html. Index.html is the main (Stock search and top 10 stock market data). Result.html gives the summary of the stock information including the  previous close, open price, Day’s range,volume, market cap and beta (all daily, besides the 52 week range and beta). We also have a css file, which is for styling the frontend. We have a virtual environment directory (.venv). Lastly, the python cache directory, the file that is automatically generated by python. 
4.      Collaborations: Julian and Young, we both met at the library at least twice a week to work on the project. We mostly used Young’s computer to work on the project. On the first meeting, we started off with designing the web. At first, we tried to copy the yahoo finance web design, but it was difficult for us to design with our capabilities. Therefore, we just decided to offer the simple design yet information that is specifically tailored to the individual traders rather than the corporations.
5.    Acknowledgements:
yfinance API - Allow us to fetch the stock data and information
Flask - Enable Python compatibility 
Chat Gpt - Solve any problems that we faced
Matplotlib - Allow us to create the visualization (Chart/Graph) 
Plotly - Allow us to give more interactive graph 
Pandas - Convert the financial data into the data frame (Convenience) 
6. Reflections: 
	
One of the most significant challenges we face is the limitations of our coding skills. When encountering issues or bugs, particularly in integrating data into the balance sheet and cash flow statement, it often takes us hours to resolve. For instance, we recently believed we had successfully fetched data for the cash flow statement, but the website displayed 'N/A' across all entries. We consulted various external resources, including Reddit, for guidance on API data implementation, but ultimately, we didn't find the solution until we realized we had a spelling error in the field name designated for essential balance sheet items. This incident underscored the importance of meticulously checking for spelling errors and other discrepancies.
The design aimed to present the required information in a clear and straightforward manner. We enhanced the user interface by implementing functional colored buttons, making it easier to navigate between documents and pages. We also tried to expand our features by including a full income statement and JavaScript functionalities, such as a tool that matches company names with their stock tickers. This allows users to enter a company name and receive corresponding ticker information, further enriching our information toolkit.
However, we encountered a setback with the API that hampered this functionality. Through these experiences, we've learned that utilizing tools like ChatGPT can be incredibly helpful in diagnosing and correcting issues. Moving forward, to avoid transcription errors, especially with API data, we plan to implement a more direct method of data entry, such as copying and pasting directly, ensuring accuracy in the characters used.


