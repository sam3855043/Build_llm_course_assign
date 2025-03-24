# Expert Knowledge Worker
A question answering agent that is an expert knowledge worker
To be used by employees of Insurellm, an Insurance Tech company
The agent needs to be accurate and the solution should be low cost.
This project will use RAG (Retrieval Augmented Generation) to ensure our question/answering assistant has high accuracy.
This first implementation will use a simple, brute-force type of RAG..

```
inport os
inport glob
from doteny import load_dotenv
import gradio as gr
from openai import OpenAI
```

```
# price is a factor for our company, so we're going to use a low cost model
MODEL = "gpt-4o-mini"
# Load environment variables in a file called ‚env
Load_dotenv ()
os. environ ['OPENAI_API_KEY'] = os-getenv( 'OPENAI_API_KEY', 'your-key-if-not-using-env' )
openai = OpenAI ()
context={}
employees = glob.g lob("knowledge-base/employees/*")
```
