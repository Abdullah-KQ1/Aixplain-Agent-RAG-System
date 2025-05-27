# Aixplain Agent RAG System Project
The Aixplain Agent is a Retrieval-Augmented Generation (RAG) agent that integrates data from three different sources to provide comprehensive answers to user queries. The system retrieves and indexes data from the following sources:

- **CSV File:** Contains detailed country information.

- **Web Scraped URL:** Provides regulatory and guidance information on air quality topics.

- **API:** Fetches real-time flight data.


The agent stores the CSV data and the scraped web data in separate index. The CSV file offers insight into various country statistics, while the web-scraped URL delivers regulatory details pertaining to air quality. Additionally, the integrated API supplies the latest flight information.

The data sources are:

- **CSV Dataset:** [Countries of the World 2023](https://www.kaggle.com/datasets/nelgiriyewithana/countries-of-the-world-2023?select=world-data-2023.csv)
    
- **Web URL:** [EPA Regulatory and Guidance Information on Air](https://www.epa.gov/regulatory-information-topic/regulatory-and-guidance-information-topic-air)
    
- **API:** [AviationStack](https://aviationstack.com/) ""



### Tool Integration Steps

1. **Query Handling:**
    - When a user submits a query, determine the relevant data source(s) based on the query topic.
    - Retrieve and aggregate information from the appropriate indices and API.
2. **Answer Generation:**
    - Utilize the RAG framework to generate clear, concise, and accurate responses by combining retrieved data with natural language generation.

### Examples

**Example 1:**
- **Input:** "What is the birth rate in Saudi Arabia?"
    
- **Output:** "The birth rate in Saudi Arabia is 17.8."


**Example 2:**
- **Input:** "Are there any EPA regulations or standards?"
    
- **Output:** "The EPA sets limits on certain air pollutants under the Clean Air Act (CAA). This includes regulations on emissions from sources such as chemical plants and utilities. Key focus areas include greenhouse gases, criteria air pollutants, and toxic air pollutants. For more detailed information, please refer to the EPA’s official resources on air quality standards and regulations."


**Example 3:**

- **Input:** "What is the latest flight information for Emirates?"
- **Output:** "The latest flight information for Emirates includes:
    - Emirates flight EK5453 from Perth International (PER) to Karratha (KTA) is currently en route.
    - Emirates flight EK5718 from Perth International (PER) to Canberra (CBR) is currently en route."

