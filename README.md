# LLMuminate.ai

LLMuminate Demo: https://youtu.be/B4zkUex2taA

Integrated real-time fact-checker for all LLM's (compatible with ChatGPT, Gemini, Claude, etc.) and all webapges. Around 45% of people in the US use LLM's like ChatGPT on a daily basis. Almost none of them fact-check what the LLM feeds them. Unfortunately, the fact of the matter is that over 50% of responses generated by LLM's are factually incorrect, especially in areas involving health and sciences. 

LLMuminate.ai is a browser extension that will fact-check LLM responses in real-time using the top 10-20 most relevant scholarly, peer-reviewed research papers from reputable journals like PubMed. We use Anthropic API to extract keywords from the LLM response, which are then formatted with boolean logic to ensure the most relevant results, and then plugged into a search on PubMed (and other journals). The resulting articles are scraped and their full text extracted. This full text is then analyzed by Anthropic API, which will extract relevant quotes and compare the information in the scholarly articles to the information given by the LLM. 

The resulting user output is a summary featuring an analysis of each of the LLM's points, and evidence (quotes) from the articles either in support of, neutral, or against what the LLM stated to be true. The links to the papers are also provided in case the user would like to explore further. 

Tech stack:

Frontend: JavaScript, HTML, CSS

Backend: Python, Flask, BeautifulSoup
