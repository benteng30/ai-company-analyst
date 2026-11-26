# AI Company Analyst

Ask plain-English questions about public companies and get answers backed by citations to their SEC filings.

> **Example:** "What are Nike's biggest supply chain risks?" → an answer citing the exact section of Nike's 10-K.

🚧 **Status: in progress** (started November 2026)

## How it will work
1. **Collect:** download annual reports (10-Ks) from SEC EDGAR
2. **Search (RAG):** split reports into passages and find the ones most relevant to a question using embeddings
3. **Agent:** an LLM chooses between tools (search the reports, query financial numbers with SQL, pull stock prices) and writes a cited answer
4. **Evaluate:** a 50-question test set to measure and improve accuracy
5. **App:** a Streamlit web app

## Progress
- [x] First LLM API call, plus a mini-RAG that answers only from given text
- [ ] Download 10-Ks from SEC EDGAR
- [ ] Embedding search over report passages
- [ ] Q&A with citations
- [ ] Agent with SQL and stock-price tools
- [ ] Test set and accuracy results
- [ ] Streamlit app

## Tech
Python · Google Gemini API · Chroma · SQLite · yfinance · Streamlit · Google Colab

## Author
Ben Teng, UMass Amherst (Isenberg, Operations & Information Management)
[LinkedIn](https://www.linkedin.com/in/ben-teng)
