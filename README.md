# Jeopardy Questions Analysis

This project analyzes a dataset of over 200,000 Jeopardy questions to uncover patterns that could help contestants prepare more effectively. The goal is to explore trends in question content, answer overlap, category frequency, and high-value vs low-value questions.

## Dataset

The dataset contains the following columns:

- **Show Number** – Episode identifier  
- **Air Date** – Date the episode aired  
- **Round** – Jeopardy, Double Jeopardy, Final Jeopardy, or Tiebreaker  
- **Category** – Question category  
- **Value** – Dollar amount of the question  
- **Question** – Text of the clue  
- **Answer** – Correct response  

Dataset source: [Reddit - Jeopardy Questions Dataset](https://www.reddit.com/r/datasets/comments/1uyd0t/200000_jeopardy_questions_in_a_json_file)

## Key Analyses

- **Text Normalization**: Cleaned and standardized question and answer text.  
- **Answer-Question Overlap**: Measured how often answer words appear in the question.  
- **Recycled Questions**: Tracked repeated words in questions across episodes.  
- **High vs Low Value Questions**: Identified terms associated with \$800+ questions using chi-squared tests.  
- **Category Patterns**: Examined top categories and their probabilities across rounds.  

## Tools

- Python (pandas, numpy)  
- SciPy (chi-squared tests)  
- Visualization: matplotlib, seaborn  

## Insights

- Only ~4% of meaningful answer words appear in the question.  
- Most questions reuse ~87% of words from previous questions.  
- Certain terms are more associated with high-value questions.  
- Category focus varies by round, with some rounds showing more predictable topics.

## Usage

Clone the repository and run the Jupyter notebook to reproduce the analyses and visualizations.

