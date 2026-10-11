# Graph Retrieval-Augmented Generation

Coursework notebooks from the DeepLearning.AI short course
[Knowledge Graphs for RAG](https://deeplearning.ai/short-courses/knowledge-graphs-rag),
created in collaboration with Neo4j and taught by Andreas Kollegger.

## Attribution

These are the course's own lesson notebooks, kept here as a record of working
through the course. The notebook text, code and structure were written by
DeepLearning.AI and Neo4j and remain their property. This repository is not
original work, and it is not affiliated with or endorsed by either organisation.

## What the course covers

Querying a graph with Cypher, then building a knowledge graph from SEC filings
in Neo4j and using it for retrieval-augmented generation with LangChain and
OpenAI models.

## Notebooks

| Lesson | Notebook | Topic |
|---|---|---|
| 2 | [query_with_cypher.ipynb](query_with_cypher.ipynb) | Querying Knowledge Graphs with Cypher |
| 3 | [prep_text_for_RAG.ipynb](prep_text_for_RAG.ipynb) | Preparing Text Data for RAG |
| 4 | [construct_kg_from_text.ipynb](construct_kg_from_text.ipynb) | Constructing a Knowledge Graph from Text Documents |
| 5 | [add_relationships_to_kg.ipynb](add_relationships_to_kg.ipynb) | Adding Relationships to the SEC Knowledge Graph |
| 6 | [expand_the_kg.ipynb](expand_the_kg.ipynb) | Expanding the SEC Knowledge Graph |
| 7 | [chat_with_kg.ipynb](chat_with_kg.ipynb) | Chatting with the SEC Knowledge Graph |

## Running them

The notebooks were written for the course's hosted environment and will not run
from this repository alone. They need:

- A Neo4j database, with `NEO4J_URI`, `NEO4J_USERNAME`, `NEO4J_PASSWORD` and
  `NEO4J_DATABASE` set in a `.env` file.
- An OpenAI API key in `OPENAI_API_KEY` (and optionally `OPENAI_BASE_URL`).
- The Python packages `langchain`, `langchain-community`, `langchain-openai`
  and `python-dotenv`.
- The course data files, which are not included here:
  `data/form10k/0000950170-23-027948.json` and `data/form13.csv`.