# CORD-19_KTool
Knowledge tool for COVID-19 papers on the CORD-19 dataset.

<div>
<img src="https://img.shields.io/badge/Python%20-%2343853D.svg?&style=for-the-badge&logo=Python&logoColor=white"/>
<img src="https://img.shields.io/badge/pandas%20-%2343853D.svg?&style=for-the-badge&logo=pandas&logoColor=white"/>
<img src="https://img.shields.io/badge/NLTK%20-%2343853D.svg?&style=for-the-badge&logo=NLTK&logoColor=white"/>
<img src="https://img.shields.io/badge/huggingface%20-%2343853D.svg?&style=for-the-badge&logo=huggingface&logoColor=white"/>
<img src="https://img.shields.io/badge/bert%20-%2343853D.svg?&style=for-the-badge&logo=bert&logoColor=white"/>
<img src="https://img.shields.io/badge/scispacy%20-%2343853D.svg?&style=for-the-badge&logo=scispacy&logoColor=white"/>
<img src="https://img.shields.io/badge/ipywidgets%20-%2343853D.svg?&style=for-the-badge&logo=ipywidgets&logoColor=white"/>
<img src="https://img.shields.io/badge/ktrain%20-%2343853D.svg?&style=for-the-badge&logo=ktrain&logoColor=white"/>
<img src="https://img.shields.io/badge/LDA%20-%2343853D.svg?&style=for-the-badge&logo=LDA&logoColor=white"/>
</div>

## Situation
Scientists have a hard time browsing through the huge amount of papers about COVID-19, and there is a lack of tools with good search interfaces to retrieve the most prominent ones for the researcher.

## Task
Devise a proof of concept 

## Action
We applied Latent Dirichlet Allocation (LDA - NLTK) to model, based on research aspects, the topics of all English abstracts in a big COVID-19 paper dataset called CORD-19. Research aspects of each paper were extracted with transformer model CODA-19, trained with data from 10k CORD-19 abstracts. Relevant named entities of each abstract were extracted and linked to the corresponding UMLS concept with SciSpacy. Regular expressions and the K-Nearest Neighbors algorithm were used to rank relevant papers.

## Results
Our tool has shown the potential to assist researchers by automating a topic-based search of CORD-19 papers. Nonetheless, we identified that more fine-tuned topic modeling parameters and increased accuracy of the research aspect classifier model could lead to a more accurate and reliable tool

[Link for arxiv paper](https://arxiv.org/abs/2401.16430)

![diagram2](https://github.com/pivettamarcos/CORD-19_KTool/assets/24397077/c127b421-d4af-4133-b1c0-055f4f092e9a)


