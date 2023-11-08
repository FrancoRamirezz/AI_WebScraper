# WebScraper, Langchain and OpenAI 🥇
## Table of Contents 🤖
- [Installations](#installations)
- [Common problems](#problems)
- [For proxy users](#proxy)
- [Future use](#Future)
## Installations 🤖:
pip install openai,
pip install langchain,
pip install playwright
from langchain.memory import ConversationBufferWindowMemory
from langchain.agents import load_tools, AgentType, initialize_agent
from langchain.document_loaders import AsyncChromiumLoader
from langchain.document_transformers import BeautifulSoupTransformer
from langchain.document_loaders import AsyncHtmlLoader
from langchain.document_loaders import WebBaseLoader

## Common issues 🎮
if there is an issue with the event loop, it could be caused by Google Colab, but it depends on the environment that you are running on.
For example, "async" works well in front of a function

## for proxy uses 💻 :
use the following code 
import request 

set_proxies = {
"https": "http://proxy1.example.com:8080",
"https": "https://proxy2.example.com:8443"",
}
response = requests.get("https://www.example.com", set_proxies=set_proxies)
print(response.status_code)
## future use 🔮: 
For the interface, it might be wise to use gradio or streamlit. If you want to use Docker here are the commands needed to run on Google Colab
'''bash
apt-get update
!apt-get install -y docker.io
!sudo dockerd &
#!docker pull hello-world
#!docker run hello-world

 
