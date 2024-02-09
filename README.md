# Topsis_Text_Generation
Text generation involves AI systems producing written content that mimics human language patterns and styles. This project aims to compare the performance of various text generation models to assist users in selecting the most suitable model for their specific requirements.

Key Features
Metrics Considered:
BLEU Scores: Measure of the quality of machine-generated text compared to human-generated text.
Model Size: The size of the model, which can impact memory and computational resources required.
Inference Time: Time taken by the model to generate text, influencing real-time applications.
Fact-checking Scores: Evaluation of generated text for factual accuracy.
Methodology - TOPSIS:
The Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) method is utilized for comparison. It considers both similarity to the ideal solution and dissimilarity to the negative ideal solution, providing a comprehensive ranking.

Models Evaluated:
T5-base
GPT-2
BLOOM
Bart Large
Jurassic-1 Jumbo
These models are prevalent in text generation tasks and are evaluated based on the mentioned metrics.

Project Structure
Data Files:
data.csv: Contains evaluation metrics for each model.
result.csv: Tabular format CSV file with ranked results.
barchart.png: Visualization of the model comparison in the form of a bar chart.
The project structure facilitates easy comparison and decision-making based on the performance metrics of the evaluated text generation models.
## Results and Analysis:
1. **Ranked Table:**
- Explore detailed ranked results in summarization_table_result.csv:

| Model            | Model_size_GB | Inference_Time_ms | BLEU_Score | Fact_Checking_Score_(0-100) | TOPSIS_Score | Rank |
| ---------------- | ------------- | ----------------- | ---------- | --------------------------- | ------------ | ---- |
| T5-base          | 0.7           | 1.5               | 37.4       | 85                          | 0.920279     | 1    |
| GPT-2            | 1.5           | 0.8               | 35.8       | 75                          | 0.458519     | 2    |
| BLOOM            | 3.9           | 2.1               | 42.1       | 82                          | 0.149159     | 4    |
| Bart Large       | 3             | 2.5               | 40.3       | 83                          | 0.202173     | 3    |
| Jurassic-1 Jumbo | 18.6          | 3.8               | 44.2       | 88                          | 0.006171     | 5    |


2. **Bar Chart:**
The bar chart visually represents the performance metrics of each model, providing an easy-to-understand comparison.
![Alt Text](barChart.png)
