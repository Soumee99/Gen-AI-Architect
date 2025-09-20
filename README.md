# Gen-AI-Architect
Projects related to Gen AI architect Program

### Project 1: Assignment: Real-Time Market Sentiment Analyzer Using LangChain Chains
#### Objective
Build a LangChain-powered pipeline (Chain) that:
1. Accepts a company name as input.
2. Extracts or generates its stock code.
3. Uses News search tools in LangChain to fetch news about the company.
4. Sends the news to an LLM (Google Gemini-2.0-flash) to generate a structured 
sentiment profile.
5. Outputs the result as a JSON object.
6. Uses mlflow for tracing, prompt debugging, and monitoring

## Set up Instructions for Google Gemini key:
1. Login to https://aistudio.google.com/prompts/new_chat
2. Click on "Get API key"
3. A Gemini API key will get generated
4. load the key in the .env file and access it.

## Set up the ML FLow Tracking URL:
1. Install MLflow.First, ensure you have MLflow installed in your environment.

   You can install it using pip:

   ``` python
   !pip install mlflow
   ```
   
3. Start the Tracking Server

Run the MLflow tracking server to establish a central location for your tracking data:

mlflow server --host 127.0.0.1 --port 8080

--host 127.0.0.1:

Specifies the IP address to bind the server to (local machine in this case). 

--port 8080

: Specifies the port number the server will listen on.

4. Set the Tracking URI

To make your MLflow client connect to the running tracking server, set the tracking URI in your Python code:
import mlflow

```python
mlflow.set_tracking_uri("http://127.0.0.1:8080")
```
