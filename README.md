## About The Project

This project has developed an UI that asks the users who are seeking for jobs their personal information and ideal job information. Based on the provided information, it will analysis the relevant job posts and the recommended best matched jobs.

### The Maching and Recommendation System

Our recommender system is data-driven and personalized. It follows the common pattern of recommender systems, which includes two steps: recalling the data and ranking them. The recalling is implemented by crawling data from websites, so here we briefly introduce the ranking part of this system.

![Structure of a recommender system. | Download Scientific Diagram](https://github.com/ryanmaomaomao/insightfo/blob/main/algorithm.png)



The ranking system is done by calculating the reciprocal matching score for a user and a job. To compare the similarity between the user experience and a job description, we have come up with a hybrid solution that utilizes two classical methods. 

The first method we came up with calculates the edit distance from the user-required job title to each of the job titles that appear in the indeed. Edit distance measures how dissimilar two strings (e.g., words) are to one another. This part ensures the job posts are roughly what users want. 

The second method uses more detailed user profiles, including working experience, education experience, and skills, to measure how close the users are matched with certain jobs.
Both parts implement a TRIE-based dynamic programming edit distance algorithm, and also tf-idf algorithm. These two algorithms together quantify the reciprocal distance between user entities and job entities.

## Getting Started

### Python Version

Python 3.9

### Prerequisites

Please see install below prerequisite libraries:

- Re - regular expression operations

- pandas, numpy, random - for basic data structures

- time, requests, bs4 - for Web scraping

- matplotlib, wordcloud - for plotting

- wx, jinja2 - UI tool
- Sklearn.feature_extraction.text - for feature extraction

## Usage

1. Run login.py
2. Enter ideal job information for job searching
3. Enter personal information for job matching
4. See report in result.html

### Video Demo

Check out our demo video link at [here](https://github.com/ryanmaomaomao/insightfo).

## Contact

Yihan Cao - yihanc@andrew.cmu.edu

Yicen Ma - yicenm@andrew.cmu.edu

Yilin Cao - yicenm@andrew.cmu.edu

Xinming Jiang - xinmingj@andrew.cmu.edu

Shuyi Chen - shuyic@answer.cmu.edu
