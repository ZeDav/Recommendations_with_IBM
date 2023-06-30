# Recommendations_with_IBM
Possible solution of the Udacity Data Science Nanodegree Project 3: Building a Recommender Engine

## Table of Contents
1. [Introduction](#introduction) 
2. [Project Overview](#overview)
3. [File Descriptions](#files)
4. [Installation](#installation)
5. [Acknowledgements](#acknowledgements) 
5. [License](#license) 

## Introduction: <a name="introduction"></a>
Building a Recommender Engine in collaboration with IBM. In this project the interactions that users have with articles on the IBM Watson Studio platform will be analyzed. Based on that a recommendation engine is build which recommends new articles to users what might be in their interest. In order to determine which articles should be recommended a study on the available data on IBM Watson Studio platform was performed. The actual work was done in a provided workspace. ([Udacity](https://www.udacity.com/)

## Project Overview: <a name="overview"></a>

#### i. Exploratory Data Analysis<br/>
Before making recommendations of any kind, you will need to explore the data you are working with for the project. Dive in to see what you can find. There are some basic, required questions to be answered about the data you are working with throughout the rest of the notebook. Use this space to explore, before you dive into the details of your recommendation system in the later sections. ([Udacity](https://www.udacity.com/))
#### ii. Rank Based Recommendations<br/>
To get started in building recommendations, you will first find the most popular articles simply based on the most interactions. Since there are no ratings for any of the articles, it is easy to assume the articles with the most interactions are the most popular. These are then the articles we might recommend to new users (or anyone depending on what we know about them). ([Udacity](https://www.udacity.com/))
#### iii. User-User Based Collaborative Filtering<br/>
In order to build better recommendations for the users of IBM's platform, we could look at users that are similar in terms of the items they have interacted with. These items could then be recommended to the similar users. This would be a step in the right direction towards more personal recommendations for the users. You will implement this next. ([Udacity](https://www.udacity.com/))
#### v. Matrix Factorization<br/>
Finally, you will complete a machine learning approach to building recommendations. Using the user-item interactions, you will build out a matrix decomposition. Using your decomposition, you will get an idea of how well you can predict new articles an individual might interact with (spoiler alert - it isn't great). You will finally discuss which methods you might use moving forward, and how you might test how well your recommendations are working for engaging users. ([Udacity](https://www.udacity.com/))
## File Descriptions: <a name="files"></a>
```
Recommendations_with_IBM /
│
├── data/
│   ├── articles_community.csv # Articles on the IBM Wotson Studo platform
│   ├── user-item-interaction.csv # List of articles users interact
│
├── LICENSE
├── README.md
├── Recommendations_with_IBM-zh.ipynb
├── Recommendations_with_IBM.html 
├── Recommendations_with_IBM.ipynb # all the work done in here
├── project_test.py # Contains solutions to for provided test questions in the Jupyther Notbook
├── top_10.p # P file with the top 10 articles (p files are uses by project_test.py)
├── top_20.p # P file with the top 20 articles
├── top_5.p# P file with the top 5 articles
├── user_item_matrix.p # User item matrix to perform Singular Value Decomposition (SVD)
```

## Installation: <a name="installation"></a>
Everything needed to complete the project is provided in the workspace, including starter files, testing advice, and instructions. 
Python 3  was used in the Jupyther Notebook

### Libraries Used
pandas, numpy, matplotlib, pickle

## Instructions: <a name="instructions"></a>
Run the codes inside Jupyther notebook to complete the project.

## Acknowledgements: <a name="acknowledgements"></a>
* [Udacity](https://www.udacity.com/) for providing Data Scientist training program.
* [IBM](https://www.ibm.com/) for providing the dataset from IBM Watson Studio.
*[Stackoverflow]( https://stackoverflow.com/) for appriciatable hinks to solve the task. 

## License: <a name="license"></a>

MIT License

Copyright (c) 2023 ZeDav

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
