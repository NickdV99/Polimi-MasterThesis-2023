# Polimi-MasterThesis-2023

# Prompt Engineering and Response Evaluation: Unveil the Dynamics of Large Language Models

## Abstract

Large Language Models (LLMs) have become integral components in various applications, ranging from natural language understanding to content generation. As their significance grows, so does the need to scrutinize and evaluate their responses due to potential risks such as private data leaks and the generation of inappropriate, harmful, or misleading content.

This master’s thesis delves into the assessment of Large Language Models responses, introducing key metrics such as correctness, coherence, relevance, and completeness. Recognizing that the quality of responses is intricately linked to the nature of the questions posed to Large Language Models, we explore the concept of prompt engineering as a crucial factor influencing response quality.

To conduct a comprehensive evaluation, we utilize multi-domain datasets as well as domain-specific ones, encompassing both open-answer and multiple-choice formats, in order to ensure an unbiased and generalized evaluation. Our analysis reveals intriguing findings, demonstrating that the effectiveness of prompt engineering is not universal. While in certain cases, optimizing prompts enhances response quality, in others, it introduces unnecessary complexity, leading to inferior results.

## Table of Contents

- [Statement of the Problem](#statement-of-the-problem)
- [Research Objectives](#research-objectives)
- [Thesis Structure](#thesis-structure)

## Statement of the Problem

In the ever-evolving landscape of computer engineering, the advent of Large Language Models (LLMs) has ushered in a new era, where these sophisticated models play a pivotal role in a myriad of applications. From unraveling the nuances of natural language to generating content with remarkable finesse, LLMs have become integral components across various domains. Their significance is underscored by their omnipresence in tasks ranging from language understanding to content creation. As these models permeate deeper into our technological fabric, the imperative to scrutinize and evaluate their responses becomes increasingly pronounced.

The crux of our research lies in acknowledging the inherent challenges that accompany the deployment of LLMs. The exponential growth in their utility brings forth potential risks, such as private data leaks and the inadvertent generation of inappropriate, harmful, or misleading content. This necessitates a comprehensive investigation into the quality of responses produced by LLMs, laying the foundation for our exploration into the intricate interplay between these models and the questions posed to them.

## Research Objectives

The overarching objective of this master's thesis is to provide a nuanced understanding of the quality of responses produced by Large Language Models, particularly in the face of varying questions. Specific objectives include:

- To introduce and define key metrics such as correctness, coherence, relevance, and completeness for assessing the quality of Large Language Models responses.
- To explore the impact of prompt engineering on the quality of responses and discern the conditions under which it is effective or counterproductive.
- To utilize datasets of different types and from various domains in order to have unbiased and universal results.

## Thesis Structure

The structure of this thesis unfolds in a logical progression, mirroring the intricacies of our exploration into LLM responses and prompt engineering. Following this introduction, the subsequent sections include:

1. **State of the art:** A comprehensive survey of existing literature, exploring the evolution of LLMs, their applications, and the state of research in evaluating response quality.
  
2. **Methodology:** A detailed exposition of our research methodology, outlining the strategies employed in assessing correctness, coherence, relevance, and completeness. This section also delves into the datasets used, the rationale behind their selection, and the prompt engineering methods adopted to improve response quality.
  
3. **Experiments:** In this section, we describe the experiments conducted to evaluate the impact of prompt engineering on LLM responses. We detail the setup, parameters, and conditions of our experiments to provide transparency and repeatability.
  
4. **Results analysis:** A presentation and analysis of the intriguing findings gleaned from our comprehensive evaluation, shedding light on the nuances of prompt engineering and its impact on response quality.
  
5. **Conclusion:** A succinct summary of our research, encapsulating the key takeaways, contributions, and avenues for future exploration.

## Usage

This repository contains the colab notebooks for running experiments, analyzing results, and visualizing data related to prompt engineering and response evaluation in Large Language Models.

### Experiment Notebooks:

- [Evaluation of Correctness Race - high.ipynb](Evaluation%20of%20Correctness%20Race%20-%20high.ipynb)
- [Evaluation of Correctness Race - middle.ipynb](Evaluation%20of%20Correctness%20Race%20-%20middle.ipynb)
- [Evaluation of Correctness math_qa.ipynb](Evaluation%20of%20Correctness%20math_qa.ipynb)
- [Evaluation of Correctness medmcqa.ipynb](Evaluation%20of%20Correctness%20medmcqa.ipynb)
- [Evaluation of Text Quality Measures MedQuad-MedicalQnA.ipynb](Evaluation%20of%20Text%20Quality%20Measures%20MedQuad-MedicalQnA.ipynb)
- [Evaluation of Text Quality Measures MultiContextLongAnswer.ipynb](Evaluation%20of%20Text%20Quality%20Measures%20MultiContextLongAnswer.ipynb)

The experiments conducted in this study leverage various libraries, frameworks, and APIs, creating a comprehensive technological environment for the development and evaluation of language models. The key technologies employed are as follows:

- **Google Colab:** Google Colab is a free, cloud-based platform designed for writing and executing Python code. It offers a convenient environment, particularly well-suited for running experiments, including those related to machine learning.

- **OpenAI GPT-3.5-turbo:** GPT-3.5-turbo, developed by OpenAI, is a prominent language model within the GPT series. Renowned for its natural language processing capabilities, it serves as a crucial component in the experiments conducted.

- **Python Libraries:**
  - **datasets:** Used for loading and working with datasets.
  - **pandas:** Employed for data manipulation and analysis.
  - **random:** Utilized for generating random numbers.
  - **openai:** OpenAI's Python library facilitates interactions with the GPT-3.5-turbo API.
  - **matplotlib:** A comprehensive plotting library for creating visualizations in Python.

- **Machine Learning Models:**
  - **SBERT (Sentence-BERT):** SBERT plays an indirect role in calculating relevance scores. It is a variation of BERT, a pre-trained language model developed by Google, specifically adapted for computing dense sentence embeddings, thereby facilitating semantic similarity calculations in natural language processing tasks.

- **Additional Tools:**
  - **CountVectorizer and cosine similarity (from scikit-learn):** Utilized to calculate coherence scores by measuring the similarity between generated and ground truth answers.

## Datasets
 
- ### [medMCQA (Medical Multiple Choice Question-Answer) Dataset](https://huggingface.co/datasets/medmcqa) [Medical | Multiple Choice]

- ### [mathQA (Mathematics Question-Answer) Dataset](https://huggingface.co/datasets/math_qa) [Mathematics | Multiple Choice]

- ### [RACE (Reading Comprehension from Examinations) Dataset](https://huggingface.co/datasets/race) [General Knowledge | Multiple Choice]

- ### [Multi-Context Long Answer Dataset](https://huggingface.co/datasets/nbtpj/multi-context-long-answer-dataset) [General Knowledge | Open Answer]

- ### [MedQuad-MedicalQnA Dataset](https://huggingface.co/datasets/keivalya/MedQuad-MedicalQnADataset) [Medical | Open Answer]

## Contributors

- Author: [Nicola della Volpe]
- Advisor: [Prof. Cinzia Cappiello]

## License

This project is licensed under the [MIT License](LICENSE).
