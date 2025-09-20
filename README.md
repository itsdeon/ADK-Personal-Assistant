# ADK-Personal-Assistant
This is a sample ADK Multi Agent Personal Assistant Built on GCP. Currently it is equipped with tools for the following: Real-Time Information Search, Currency Exchange Rates, and Historical / Cultural Context  

Here's a breakdown of its capabilities based on the tools it's equipped with:

Currency Exchange Rates: It can fetch the current exchange rate between two currencies (e.g., "SGD" to "JPY"). It does this using the get_fx_rate function, which is wrapped in a FunctionTool.

Real-time Information Search: It can answer questions about current events, weather, or business hours. For these types of queries, it delegates the task to another agent, the google_search_agent, which is specifically designed to use Google Search for real-time information.

Historical and Cultural Information: It can provide deep historical and cultural details about landmarks, concepts, and places. To do this, it uses the langchain_wikipedia_tool, which is configured to search Wikipedia for detailed, encyclopedic-style answers.

In essence, the root_agent is a versatile assistant that intelligently routes a user's question to the most appropriate tool or sub-agent to get the best possible answer, whether it's a financial query, a real-time search, or a request for deep knowledge.

Testing of the Agent was done using ADK Web 
