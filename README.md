# Abstract

In the domain of natural language processing, aspect-level sentiment analysis remains a crucial yet underexplored area, particularly within the tourism industry. This study aims to address this gap by extracting aspect terms from TripAdvisor reviews, thereby identifying specific attributes discussed in these reviews. The objective is to enhance customer experiences and uncover competitive advantages within the industry. This research employs large language models  such as Google-Flan-T5-Large, Mistral-7B, and LLaMA-2-7B to evaluate their efficacy in capturing aspect nuances in tourism-related texts. To determine the most effective Large Language Model for aspect-level sequence labeling in the tourism domain, various prompting techniques are investigated, including zero-shot learning, one-shot learning and few-shot learning. Apart from these, retrieval-augmented generation, and fine-tuning were also employed. A comparative analysis of their performance on our dataset is presented, revealing that Mistral-7B achieved an accuracy of  91% and a macro F1-score of 70%.


# Proposed Methodology

We have employed three techniques to extract aspect terms- prompting techniques like zero-shot, one-shot etc, RAG and fine-tuning of LLMs as depicted by the system architecture in Fig. 4. to compare these techniques to see which leads to a more accurate result for extracting aspect terms. The final step involves assessing the performance of the models, using the metric Macro F1 Score, which is a balanced measure of precision and recall across all classes.

<img width="484" alt="Screenshot 2024-07-15 at 12 49 24 AM" src="https://github.com/user-attachments/assets/da1a4ccf-a2e5-416b-846b-afdd8eefe681">
