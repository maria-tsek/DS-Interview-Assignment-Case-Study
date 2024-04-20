# DS-Interview-Assignment-Case-Study

<img width="992" alt="Screenshot 1" src="https://github.com/maria-tsek/DS-Interview-Assignment-Case-Study/assets/141243211/47d3132c-a89d-4852-9570-41bf8e7bc588">
<img width="1031" alt="Screenshot 2" src="https://github.com/maria-tsek/DS-Interview-Assignment-Case-Study/assets/141243211/d4d14011-3799-4a27-ad8b-a14be85dabcf">


Based on the images above, it's evident that the keyword with the highest number of searches for each search engine is what I've defined as "rank 1". This implies that for every search engine, the keyword with the highest search volume is considered as the top-ranked keyword. Therefore, the analysis provides insights into the search volume distribution across different search engines, highlighting the popularity of specific keywords within each platform.


**Observations about the Data:**
The dataset comprises five columns, each offering valuable insights into keyword performance and search behavior:

**keyword_id:** This column serves as a unique identifier for each keyword. It is notable that multiple entries exist for each keyword, implying that the dataset captures the keyword's performance across various parameters and time periods. This identifier facilitates the tracking and analysis of individual keywords' performance trends.

**keyword_rank:** The keyword_rank column signifies the relative position of each keyword in terms of its popularity or relevance. Keywords are likely ranked based on factors such as search volume, click-through rate, or relevance to a particular topic. 

**date:** The date column denotes the specific date associated with each data entry, ranging from 7/8/2022 to 7/14/2022. This temporal dimension allows for the tracking of keyword performance variations over time. Analysis of keyword trends across different dates can reveal patterns, seasonality, or sudden shifts in user behavior, aiding in strategic decision-making.

**searches:** The searches column quantifies the number of searches conducted for each keyword on a given date. It provides valuable quantitative data regarding the popularity and demand for specific keywords over time. By analyzing search volumes, we can identify trends, fluctuations, or spikes in user interest, offering insights into keyword performance dynamics.

**search_engine:** This column categorizes the search engine where the searches were executed, such as Google, Bing, or Yahoo. Distinguishing between searches performed on different platforms enables us to discern user preferences and behaviors across various search engines. Understanding the distribution of searches across different platforms facilitates targeted optimization strategies and enhances overall search engine visibility.

* *By comprehensively analyzing these columns, we can derive actionable insights into keyword performance trends, user behavior patterns, and search engine dynamics, ultimately informing strategic decisions and optimizing digital marketing efforts.* *

**What you attempted and why**
My primary objective in addressing each question is to thoroughly comprehend the dataset provided. Upon examination, it becomes evident that the dataset pertains to the week of July 2022. Notably, each keyword_id appears multiple times in the dataset, each instance associated with distinct keyword_rank, date, searches, and search_engine values.

To gain insights into the data relationships, I utilized various visualization techniques. For instance, employing a scatter plot allowed me to explore the relationship between searches and search_engine. Through this analysis, I identified the search_engine with the highest search volume, which corresponds to index 11.

Furthermore, to streamline the analysis and focus on key insights, I opted to extract a subset of the data. Leveraging Python's capabilities, I generated a list containing the most searched keyword_ids for each search engine and date. By working with a reduced dataset, I aimed to enhance clarity and facilitate more effective analysis and visualization.

Subsequently, I utilized this refined dataframe to determine the most searched keyword_id ( keyword with rank 1) for each search_engine, spanning from search_engine index 0 to 25, as outlined in the provided code snippet.

* *By adopting this systematic approach, I aim to uncover valuable insights and patterns within the dataset, enabling informed decision-making and strategic optimization of digital marketing efforts.* *

**The visualizations you used to understand the data**

**2D Histogram (Heatmap) and Scatter Plot:** Utilizing a 2D histogram (heatmap) and a scatter plot, I explored the relationship between search_engine and searches. These visualizations provided a comprehensive overview of search volume distribution across different search engines. By visualizing the data in this manner, I was able to identify patterns, trends, and potential outliers, thereby enhancing my understanding of search behavior.

**Temporal Distribution of Maximum Searches:** To examine the temporal distribution of maximum searches and their associated keyword_ids, I created a plot showcasing the date with the highest searched keyword_id. This visualization revealed that the date 11/7/2022 exhibited the highest search activity, offering valuable insights into temporal search trends and user behavior patterns.

**Maximum Searches and Corresponding Keyword ID by Search Engine:** Another visualization depicted the maximum searches and corresponding keyword ID for each search engine. This plot highlighted search engine 11 as having the highest search activity, providing valuable insights into search engine performance and user engagement across different platforms.

**3D Plot:** This plot visualizes the number of searches received by the keyword with the maximum searches for each search engine on each date. It utilizes a 3D bar chart where the x-axis represents the search engine, the y-axis represents the date, and the z-axis represents the number of searches. This plot could be a sugestion because it helps identify which keywords are most popular on specific dates and search engines, providing valuable insights into user behavior and preferences. Additionally, the use of colors and legends makes it easier to interpret the data and compare different keywords across multiple search engines.

* *By leveraging these visualizations, I was able to extract meaningful insights from the dataset, including patterns, trends, and relationships between key variables. These visualizations serve as powerful tools for understanding and interpreting the data, ultimately informing strategic decision-making and optimization efforts.* *

**Model(s) and evaluation**

Sorting Data: Initially, I sorted the dataset based on the 'searches' column in descending order.
Grouping and Aggregating: I grouped the data by 'search_engine' and found the row with the maximum 'keyword_rank' in each group. This allowed me to identify the keyword with rank 1 for each search engine.
Selection of Relevant Columns: After grouping the data, I selected the 'keyword_id' and 'searches' columns to obtain the necessary information for analysis.
Evaluation of Results:

The accuracy and reliability of the analysis were ensured through several steps:

Visualization: Visualizations such as scatter plots, histograms, and bar plots were used to explore the relationships between different variables and validate the results obtained from data manipulation.
Comparison with Raw Data: The results were cross-validated by comparing them with the raw data. This helped ensure that the aggregated values align with the original dataset.
Statistical Analysis: Descriptive statistics and correlation analysis were performed to assess the consistency and coherence of the results.
Domain Knowledge: Domain-specific knowledge and understanding of search engine behavior were applied to interpret the results and verify their relevance and accuracy.

* *By employing these methods and evaluation techniques, I was able to derive meaningful insights and ensure the accuracy and reliability of the analysis results.* *

**Conclusions**

Based on the analysis conducted, several key conclusions can be drawn:

**Keyword Rank and Searches:** The relationship between keyword rank and the number of searches is evident, with higher-ranking keywords generally receiving more searches. This indicates that keyword rank plays a crucial role in determining search engine visibility and user engagement.

**Search Engine Performance:** The analysis reveals variations in search engine performance, with certain search engines driving higher search volumes compared to others. Understanding these differences can help optimize marketing strategies and target specific search engines for better visibility and reach.

**Temporal Trends:** The temporal distribution of maximum searches and corresponding keyword IDs provides insights into search trends over time. Identifying peak search periods can inform decision-making regarding campaign timing and resource allocation.

**Search Engine Optimization (SEO):** Insights gained from the analysis can inform SEO strategies by highlighting keywords and search engines with the highest potential for visibility and traffic generation. This knowledge can guide content creation, keyword targeting, and website optimization efforts.

**Data-Driven Decision Making:** By leveraging data analytics techniques, businesses can make informed decisions to enhance their online presence and maximize search engine visibility. Regular monitoring and analysis of search engine performance metrics are essential for staying competitive in the digital landscape.
