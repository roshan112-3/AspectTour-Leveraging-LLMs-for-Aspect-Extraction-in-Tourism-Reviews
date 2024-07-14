# Abstract

In the domain of natural language processing, aspect-level sentiment analysis remains a crucial yet underexplored area, particularly within the tourism industry. This study aims to address this gap by extracting aspect terms from TripAdvisor reviews, thereby identifying specific attributes discussed in these reviews. The objective is to enhance customer experiences and uncover competitive advantages within the industry. This research employs large language models  such as Google-Flan-T5-Large, Mistral-7B, and LLaMA-2-7B to evaluate their efficacy in capturing aspect nuances in tourism-related texts. To determine the most effective Large Language Model for aspect-level sequence labeling in the tourism domain, various prompting techniques are investigated, including zero-shot learning, one-shot learning and few-shot learning. Apart from these, retrieval-augmented generation, and fine-tuning were also employed. A comparative analysis of their performance on our dataset is presented, revealing that Mistral-7B achieved an accuracy of  91% and a macro F1-score of 70%.


# Introduction 

Traditional sentiment analysis involves assessing and categorizing a text such as a review to be  positive, negative, or neutral based on the feelings or viewpoints expressed. A more fine-grained form of sentiment analysis known as aspect-based sentiment analysis (ABSA) focuses on finding and analyzing the sentiment or opinion expressed towards aspects within the text. The aspect term extraction (ATE) task, which looks for aspect keywords that are articulated in sentences, is one of the primary tasks  in ABSA. Given the considerable global influence that tourism has on the economy and culture, this study focuses on ATE on tourism reviews from a popular website, TripAdvisor. Tourism organizations can gain valuable insights into the aspects of their offerings that tourists find most or least appealing by carefully examining customer feedback. In ABSA, aspect term extraction involves sequence labeling which is the task of assigning a categorical label to each token of a sentence.

Example review: The water rides were fun, but the land rides were boring! <br> 
Aspect Terms: [‘water rides’, ‘land rides’]

In the above review, two opinions or sentiments are being expressed on two different aspects. These terms represent specific features or components of the amusement park being reviewed. Extracting these aspect terms is important because it allows us to focus on the sentiment expressed towards each specific feature, rather than the text as a whole. 


# Proposed Methodology

We have employed three techniques to extract aspect terms- prompting techniques like zero-shot, one-shot etc, RAG and fine-tuning of LLMs as depicted by the system architecture in Fig. 4. to compare these techniques to see which leads to a more accurate result for extracting aspect terms. The final step involves assessing the performance of the models, using the metric Macro F1 Score, which is a balanced measure of precision and recall across all classes.

<img width="484" alt="Screenshot 2024-07-15 at 12 49 24 AM" src="https://github.com/user-attachments/assets/da1a4ccf-a2e5-416b-846b-afdd8eefe681">
