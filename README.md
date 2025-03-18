# DAT_RAG_LLM
DAT_RAG_LLM is a Retrieval-Augmented Generation (RAG) pipeline developed as part of a research study, to enhance 4 Large Language Models (LLMs) medical diagnostic accuracy.

## What is DAT_RAG_LLM?
This RAG pipeline integrates 62 medical text books from the [Hershey Medical School curriculum](https://harrell.library.psu.edu/Textbook) with four state-of-the-art LLMs—GPT-3.5, GPT-4o, Llama3-8b, and Gemini 1.5 Pro to generate medical diagnoses using crowdsourced health-related queries (patient cases).
By grounding the LLMs' responses in this verified medical knowledge, RAG could enhance LLMs accuracy by addressing limitations such as outdated information or lack of context. 

## Research methodology
<img
  src="https://bonam-m.github.io/DAT_RAG_LLM/datrag-process.jpg"
  alt="DAT_RAG_LLM"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 200px">  

### What can you find in this repo?
Here is a description of the content of this repository.

#### Python Notebook to convert medical books from PDF to txt
In this notebook, you will find the script to convert PDF files with images to text using GPU for fast processing.
(See _dat-pdf-books-to-txt.ipynb_)

#### Python Notebook for the 4 RAG-enhanced LLMs pipeline
In this notebok, you will find the RAG-enhanced LLMs pipelines for GPT-3.5, GPT-4o, Llama3-8b, and Gemini 1.5 Pro (see _dat-rag-pipeline.ipynb_). The outputs are saved in CSV files. 
You need API keys added to your environment to run the notebook locally.

#### Python Notebook to save LLMs output in PDF files
In this notebook, you will find the script to save the RAG-enhanced LLMs outputs in PDF files.
This step was needed in our research study, to have those outputs evaluated by physicians and medical professionals.
(See _csv-diagnoses-to-pdf.ipynb_)