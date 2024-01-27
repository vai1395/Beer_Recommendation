# Business-Oriented Beer Recommendation System

In this innovative data science initiative, we introduce a sophisticated beer recommendation system leveraging advanced sentiment analysis through Language Models (LLMs). Our goal is to distill valuable insights from the vast realm of online conversations, focusing on business-friendly attributes for a comprehensive beer recommendation experience.

## Data Source
Our dataset is meticulously curated from discussions on a reputable beer forum - [BeerAdvocate](https://www.beeradvocate.com/beer/top-rated/). This dataset undergoes rigorous preprocessing and cleaning to ensure its relevance and reliability in driving business-oriented recommendations.

## Approach
Our recommendation engine employs similarity scores between user-selected attributes and forum comments. We prioritize comments with high similarity scores and positive sentiment. The fusion of similarity scores and sentiment values is achieved through the formula:

$$ final_score = log₂(sentiment) * log₂.₅(similarity) $$

The final_scores are aggregated to the product level and a new_final_score is calculated using the avg_final_score and #comments (after all the filters) as - 

$$ new_final_score = log(no. of comments) * (log₂(avg_final_score)/log(1.5)) $$

The top three recommended beers are based on this new final score.

## Implementation
Our Python 3 code, encapsulated in the Jupyter notebook [Final Submission/Final Notebook_V3.0.ipynb.ipynb]([path/to/notebook](https://github.com/vai1395/Beer_Recommendation/blob/main/Final%20Submission/Final%20Notebook%20V3.0.ipynb)), utilizes renowned data analysis libraries including pandas, numpy, scikit-learn, nltk, openai, spacy, and selenium. The notebook is structured to facilitate easy comprehension, with sections covering data loading, preprocessing, exploratory data analysis, and model building.

## Results and Analysis
Beyond the recommendation aspect, our analysis delves into the nuances of employing word embeddings for similarity computation in Natural Language Processing (NLP). Additionally, we explore the effectiveness of LLMs compared to VADER in discerning human sarcasm during sentiment analysis, utilizing OpenAI.

All findings, results, and comprehensive explanations are encapsulated within the notebook, providing a valuable resource for business-oriented insights.

## Business Implications
This project unveils previously undiscovered insights within the beer recommendation domain.To further enhance your understanding, we have incorporated relevant images and visualizations in the notebook to convey complex information in a visually appealing manner.
