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
Devise a proof of concept tool that incorporates, in a novel way, aspects of Information Retrieval (IR) and Extraction (IE) applied to the COVID-19 Open Research Dataset (CORD-19). The main focus of this work is to provide researchers with a better search tool for COVID-19 related papers, helping them find reference papers and highlight relevant entities in text

## Action
We applied Latent Dirichlet Allocation (LDA - NLTK) to model, based on research aspects, the topics of all English abstracts in a big COVID-19 paper dataset called CORD-19. Research aspects of each paper were extracted with transformer model CODA-19, trained with data from 10k CORD-19 abstracts. Relevant named entities of each abstract were extracted and linked to the corresponding UMLS concept with SciSpacy. Regular expressions and the K-Nearest Neighbors algorithm were used to rank relevant papers.

## Results
Our tool has shown the potential to assist researchers by automating a topic-based search of CORD-19 papers. Nonetheless, we identified that more fine-tuned topic modeling parameters and increased accuracy of the research aspect classifier model could lead to a more accurate and reliable tool

### Use case diagram

[Link for arxiv paper](https://arxiv.org/abs/2401.16430)

![diagram2](https://github.com/pivettamarcos/CORD-19_KTool/assets/24397077/c127b421-d4af-4133-b1c0-055f4f092e9a)

### Example use case 1
List of COVID-19 abstracts whose finding/contribution addresses the topic “patients, day, median, hospital, iqr, admission, range, died and years”, ordered by date of publication
![admission](https://github.com/pivettamarcos/CORD-19_KTool/assets/24397077/205d1a17-8d0c-498b-bcf6-62a86c5d6bb6)

### Example use case 2
List abstracts whose background addresses the topic of environmental stability of the virus
![environmental](https://github.com/pivettamarcos/CORD-19_KTool/assets/24397077/bad18376-243b-402e-a583-195f3ab5ad80)
 
### Example use case 3
Individual abstract visualization, with research aspects highlighted in different colors and UMLS terms visible to the user
![single_abstract](https://github.com/pivettamarcos/CORD-19_KTool/assets/24397077/9e1cff3a-22b8-4b8c-b063-19c304399ea4)


