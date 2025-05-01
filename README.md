# GlucoGuide
LLM-Powered Blood Sugar Insights

## Purpose
To build hands-on experience with large language models and AI tools commonly used in industry, while creating a useful product for people with diabetes. This project will demonstrate the abilit to integrate time-series data, domain-specefic knowledge, and generative AI for personalized health insights

## Core Features 

1. Interactive Dashboard: Select a timeframe (1 week to 1 year) to visualize blood sugar patterns.

2. Ambulatory Glucose Profile (AGP) Chart: Display glucose percentiles (median, 25%, 75%, 50%, 95%) collapsed into a 24-hour day view.

3. LLM-Powered Chatbot: Analyze AGP and surface trends (e.g., morning lows) with suggestions (e.g., adjust background insulin). The LLM chatbot automatically refreshes its analysis using only the data from the timeframe selscted.

4. Personalized Insights: Use structured rules and LLM reasoning to interpret patterns and explain them in accessible language. Allow users to ask questions regarding the selected time frame. 

## Tech Stack (Tentative)

Front end: Potentially streamlit dashboard development

Backend/Modeling: Python, Pandas, NumPy, PyTorch or TensorFlow

LLM Integration: OpenAI API or Hugging Face Transformers

Data Visualization: Plotly or Matplotlib

Optional: LangChain for LLM pipelines

## Data Source

The core data for this project will come from my own Dexcom Clarity exports. Dexcom Clarity provides downloadable reports in CSV or PDF format that include:

Timestamps of glucose readings (every 5 minutes)

Glucose levels (in mg/dL)

Daily summaries including average glucose, time in range, and standard deviation

These data will enable calculation of the Ambulatory Glucose Profile (AGP) by aggregating glucose readings over a selected timeframe and mapping them into a 24-hour distribution.
