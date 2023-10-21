
# WebScraper, Langchain and OpenAI
# Installations:
pip install openai,
pip install langchain,
pip install playwright
from langchain.memory import ConversationBufferWindowMemory
from langchain.agents import load_tools, AgentType, initialize_agent
from langchain.document_loaders import AsyncChromiumLoader
from langchain.document_transformers import BeautifulSoupTransformer
from langchain.document_loaders import AsyncHtmlLoader
from langchain.document_loaders import WebBaseLoader
# Common Problems
