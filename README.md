# Japanese-American Incarceration Oral History Analysis

## Overview

We are at a crucial juncture in history, where the stories of our ancestors, preserved in various formats, are increasingly accessible. Historically, archiving was a manual process managed by archivists, which proved to be time-consuming. However, with the rise of digital technology, there is an urgent need for automation and digitalization [1].

This project addresses this challenge by exploring solutions and tools for effective digital archiving. Our focus is on applying **Natural Language Processing (NLP)** and **Machine Learning (ML)** models to the history of Japanese-American Incarceration. We will analyze four online collections: the Densho repository, the Japanese American Service Committee (JASC), the Japanese American Museum of San Jose (JAMSJ), and Discover Nikkei. Our research aims to answer the following questions:

1. **What are the narrators' descriptions**, including their nationality, race, age, and birthplace?
2. **Are there common characteristics or points** among each incarceration camp?
3. **What activities or significant events** are associated with individuals mentioned by multiple narrators?

Our objective is to extract valuable insights and contextual information from these methods.

## Data Analysis Plan

We will use a range of NLP and ML techniques to extract insights from the oral history data. The main steps include:

- **Descriptive Analysis**: Extracts information such as narrator’s name, generation, nationality, birth year, birth place, and camp location. This step includes creating distribution visualizations to address the first research question.

- **Entity Extraction**: Captures additional entities such as organizations, facilities, languages, dates, and years. This step, in conjunction with sentiment analysis and topic modeling, helps answer the second and third research questions. It also allows for specific subject analysis by creating subsets from these entities.

- **Annotation Scheme**: Defines seven major categories related to Japanese American Incarceration history. This scheme helps classify all transcript data into these categories, facilitating more focused analysis. It is used in conjunction with text classification and is foundational for further analysis.

- **Text Classification**: Labels and classifies all text data into the seven categories defined by the annotation scheme. This method enables organized data analysis and focused examination of categorized topics.

- **Sentiment Analysis**: Computes sentiments from text data to understand Japanese Americans' feelings about the seven topics or other specific subjects. This analysis helps address the second and third research questions.

- **Topic Modeling**: Identifies subtopics within the main categories, highlighting keywords and relationships. This method provides a detailed understanding of each topic and complements sentiment analysis by offering insights into subtopics and keyword associations.

## Research Structure

The research paper is organized as follows:

1. **Related Work**: Reviews 23 research papers relevant to our subject, highlighting useful methods for our analysis.
2. **Data Collection**: Describes the processes of obtaining, cleaning, and preprocessing data using computational methods.
3. **Methodologies**: Provides detailed explanations of the tools, methods, and analyses used in the main tasks.
4. **Results and Discussion**: Presents and discusses results with multiple visualizations.
5. **Conclusion and Limitations**: Summarizes the research findings and outlines any limitations.

## Figures

- **Fig.1**: Overview of the research processes.

We aim to unlock valuable insights and context within the oral history transcripts to better understand the history of Japanese-American Incarceration.
