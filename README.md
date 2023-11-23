# FinSight-AI-Analyzer
# Introduction
FinSight is an advanced and user-friendly news research tool, meticulously designed to streamline and enrich the process of extracting information from news articles, with a special focus on the financial and stock market sectors. Integrating leading-edge technologies such as LangChain's UnstructuredURL Loader, OpenAI's sophisticated embeddings, and the FAISS similarity search library, FinSight emerges as a powerful tool for professionals and enthusiasts seeking prompt, reliable, and comprehensive analysis of financial news
![](Interface.jpg)

##Features
Advanced Article Content Loading: FinSight enables users to effortlessly input URLs or upload text files containing URLs, fetching the content of these articles for subsequent analysis. This feature is pivotal for efficiently aggregating data from diverse news sources.

Content Processing: Utilizing LangChain's UnstructuredURL Loader, FinSight adeptly processes the content of articles, ensuring the accuracy and readiness of the data for in-depth analysis.

Efficient Information Retrieval: At its core, FinSight leverages the ability to construct embedding vectors using OpenAI's advanced embeddings, combined with the FAISS similarity search library. This amalgamation ensures swift and effective information retrieval, allowing users to quickly pinpoint the most pertinent data among a vast collection of articles.

Interactive Query-Answer Interface: FinSight integrates seamlessly with the ChatGPT model, enabling users to input queries and receive detailed answers, complete with source URLs for further exploration. This interactive feature simplifies the navigation through complex financial news, offering valuable insights in an accessible format.

User-Friendly Experience: FinSight is crafted with an emphasis on user experience, boasting an intuitive interface that accommodates users with varying levels of technical expertise

##Installation
1.Clone this repository to your local machine using:

```bash
https://github.com/balasai24/FinSight-AI-Analyzer/.git
```
2.Navigate to the project directory:

3. Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
4.Set up your OpenAI API key by creating a .env file in the project root and adding your API

```bash
  OPENAI_API_KEY=your_api_key_here
```
## Usage/Examples

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```
2.The web app will open in your browser.

- On the sidebar, you can input URLs directly.

- Initiate the data loading and processing by clicking "Process URLs."

- Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

- The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.

- The FAISS index will be saved in a local file path in pickle format for future use.
- One can now ask a question and get the answer based on those news articles
  
## Project Structure

- main.py: The main Streamlit application script.
- requirements.txt: A list of required Python packages for the project.
- faiss_store_openai.pkl: A pickle file to store the FAISS index.
- .env: Configuration file for storing your OpenAI API key.
