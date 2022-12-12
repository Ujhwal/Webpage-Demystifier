# Webpage-Demystifier

Abstract
The major objective in this project is to summarize the text and to understand the current technological standards. Text summarization is always fasciation because the machine must understand the context and the sentiment behind the text. Then the algorithm must summarize the text without changing the sentiment or the context of the whole text. In this project, we have experimented with Abstractive summarization and Extractive summarization. To be more specific we have used various models with reference to each summarization and then compared their performance with their corresponding metrics. As a bonus, we have also used the wiki APIs to extract all the data from the Wikipedia webpage related to a keyword and provide the gist information of the complete webpage within the confined parameters.

1.	Introduction
Time is one of the more important factors of human life, the things a human being can achieve in a short span of time is fascinating.  If you are an engineer or a teacher of science, you should realize that there are more things you can accomplish with others helping hands towards your research. To acquire more knowledge, more information is needed to be analyzed, but due to time constraints one cannot go through all the materials.
Abstractive text summarization is a type of summarization that involves generating a new, concise summary of a text by using the most important information from the original text. Unlike extractive summarization, which simply selects and combines existing sentences from the original text, abstractive summarization involves creating new sentences that convey the same meaning as the original text. This allows the summary to be shorter and more concise than the original text, while still accurately representing its meaning. Abstractive summarization can be useful for quickly summarizing long documents or articles, as well as for creating summaries that are more easily understood by readers.
Extractive text summarization is a type of summarization that involves selecting and combining important sentences or phrases from the original text to create a summary. Unlike abstractive summarization, which involves generating new sentences to convey the meaning of the original text, extractive summarization simply selects and rearranges existing sentences from the original text. This means that the summary will be shorter than the original text, but it will still contain the same information. Extractive summarization is useful for quickly summarizing long documents or articles, and it can be especially useful for creating summaries that are easy to understand and accurately represent the original text.
There are several advantages to using text summarization, including:
Time savings: Summarizing a text can save a lot of time, especially when dealing with long documents or articles. By quickly generating a summary, you can get a good understanding of the main points without having to read the entire text.
Improved understanding: Summarizing a text can help you better understand its main points and the connections between different ideas. This can be especially useful when reading complex or technical texts.
Increased clarity: Summaries are typically shorter and more concise than the original text, which can make them easier to read and understand. This can be especially useful for readers who don't have a lot of time or who may be overwhelmed by the length of the original text.
Improved retention: Summarizing a text can help you better remember its main points. By condensing the information into a shorter, more manageable form, you can more easily retain the key ideas and concepts.



2.	Proposed Idea
•	Summarizing a website is a renowned approach which is used to reduce a webpage’s main ideas. It operates by preserving and creating a shortened version of website. 
•	In this fast-paced world, where every minute is so essential, reading the whole webpage is a time-consuming process, where we need to visit each page for a modest amount of information. By giving a weblink, this project's goal is to make information search less time-consuming. 
•	With this approach, we develop algorithms or software that will consolidate the data and produce a summary of the website. To reduce the time spent by an individual on a website searching for the actual content. Time is the most valuable asset for some people. For them, getting the essence of the large webpage is very valuable. 
•	Wiki APIs, or application programming interfaces, are used to access the contents of a wiki, which is a type of website that allows users to collaboratively create, edit, and link pages of information. These APIs can be used to extract the content of a page from a wiki and then perform text summarization on that content.
•	Performing text summarization on the results of the Wiki APIs, such that users can understand the gist of that wiki page without spending hours to completely understand the whole content. 
•	The above-mentioned process we will be implementing it for three different models, as per text summarization standpoint. We will be using different metrics like the GLUE score, cosine similarity to compare between them.
•	The three models we will be focusing throughout this project are T5, BART, Pegasus.
3.	Related Works
Text summarization is a widely studied problem in natural language processing, with a variety of approaches proposed in the literature. Some of the earliest work on text summarization focused on extractive methods, which aim to identify and select important sentences or phrases from the original text to create a condensed summary (Nallapati et al., 2016). These methods typically rely on heuristics or statistical measures to score the importance of individual sentences or words, and then select a subset of the most important sentences or phrases to include in the summary (Hannan et al., 2016; Gupta et al., 2016).
More recent work has explored abstractive summarization methods, which aim to generate new, condensed sentences that capture the main ideas of the original text (Wang et al., 2019). These methods often use neural networks and deep learning techniques, such as sequence-to-sequence models and attention mechanisms, to generate summaries that are more fluent and coherent than those produced by extractive methods (Yang, 2016; Liu et al., 2019).
Evaluating the performance of text summarization methods is a challenging task, due to the subjectivity of summarization and the lack of ground truth summaries for many texts (Al-Taani, 2017). Several evaluation metrics have been proposed in the literature, such as ROUGE and BLEU, which measure the overlap between the generated summary and a reference summary (Moratanch and Chitrakala, 2016).

4.	Technical Standards
Currently, there are several techniques used for text summarization, including extractive methods, which involve selecting important sentences or phrases from the original text, and abstractive methods, which involve generating a summary that is a condensed version of the original text. Both methods often use natural language processing and machine learning techniques to identify and select important information from the text.

Some of the most commonly used algorithms for text summarization include the TextRank algorithm, which uses graph-based ranking to identify important sentences in the text, and the Latent Semantic Analysis (LSA) algorithm, which uses singular value decomposition to identify the most important words and phrases in the text.

T5, or Text-To-Text Transfer Transformer, is a large-scale multi-lingual language model developed by Google. One of the applications of T5 is text summarization, where it can be used to generate concise summaries of longer text documents. T5 uses a transformer-based architecture, which allows it to process input text and generate output text in a variety of different languages. For text summarization, T5 is typically trained on a large dataset of input and output text pairs, where the input text is a longer document, and the output text is a summary of that document. Once trained, T5 can be used to summarize new text by providing the model with the input text and specifying the desired length of the output summary. T5 will then generate a summary that is a condensed version of the input text, while still preserving the important information and main ideas.
BART, or Denoising Sequence-to-Sequence Pre-training for Natural Language Generation, Summarization, Translation, and Dialog, is a large-scale language model developed by Facebook AI. One of the applications of BART is text summarization, where it can be used to generate summaries of longer text documents. BART is a denoising autoencoder, which means that it is trained to generate output text that is like the input text, but with certain elements removed or "masked out". For text summarization, BART is typically trained on a large dataset of input and output text pairs, where the input text is a longer document, and the output text is a summary of that document. Once trained, BART can be used to summarize new text by providing the model with the input text and specifying the desired length of the output summary. BART will then generate a summary by "denoising" the input text, removing unnecessary words and phrases while still preserving the important information and main ideas.
Pegasus is a large-scale language model developed by OpenAI. It was specifically designed for natural language generation tasks, such as text summarization, machine translation, and text-to-speech. Pegasus is based on a transformer-based architecture, which allows it to process input text and generate output text in a variety of different languages. For text summarization, Pegasus is typically trained on a large dataset of input and output text pairs, where the input text is a longer document, and the output text is a summary of that document. Once trained, Pegasus can be used to summarize new text by providing the model with the input text and specifying the desired length of the output summary. Pegasus will then generate a summary that is a condensed version of the input text, while still preserving the important information and main ideas.
5.	Methodologies
For the three models we are using similar approach to perform text summarization. Initially we will be building a pipeline, the major constituents of the pipeline include the model we intend to use for that pipeline and then the device which we want to use for the compute process. Based on these two the pipeline’s setup will be completed for the three models. 
We were using the news summary dataset from Kaggle to get the summarization text. This dataset mainly includes columns like News Headlines, which we have basically used as cross reference point for the text summarization. We also have News Text column, where it goes into the respective model pipeline for generating the text summarization.
Each of the record, contains a News Text and News Headline. Where we predict the text summarization based on the model and then saved the end results to the corresponding record in the same pandas dataframe. We have used GLUE and cosine similarity as metrics for comparing the three used models. 
6.	Results
The cosine similarity score measures the similarity between two vectors. In this case, the vectors could represent the outputs of different text summarization models, such as BART, Pegasus, and T5.  A higher cosine similarity score indicates that the vectors are more similar, while a lower score indicates that they are less similar. In the given example, the cosine similarity scores of BART, Pegasus, and T5 are 0.54043, 0.54381, and 0.62276, respectively.  This indicates that the output of BART is more like the output of Pegasus than the outputs of T5. This suggests that T5 may be more like BART and Pegasus in terms of the summary it generates, while BART and Pegasus may generate more distinct summaries.
The GLUE score, or the General Language Understanding Evaluation score, is a metric for evaluating the performance of natural language processing models. It is calculated by comparing the model's output to human-generated reference outputs on a variety of different natural language understanding tasks, such as sentiment analysis and text classification. In the given example, the GLUE scores of BART, Pegasus, and T5 are 0.03845, 0.03638, and 0.04850, respectively. This indicates that T5 has the highest GLUE score, while BART has the lowest score. A higher GLUE score indicates that the model is performing better on the natural language understanding tasks included in the evaluation. Therefore, in this case, T5 is performing better than BART and Pegasus on these tasks.

7.	References

[1] Moratanch, N. and Chitrakala, S. (2016) ‘A survey on abstractive textsummarization’, In proceedings of International Conference on Circuit, Power and Computing Technologies (ICCPCT), Nagercoil, India, pp.1-7.
[2] Wang, D., Zhu, S. and Li, T. (2013) ‘SumView: A Web-based engine for summarizing product reviews and customer opinions’, Expert Systems with Applications, Volume 40, Issue 1, pp. 27-33.
[3] Yang, L. (2016) ‘Abstractive Summarization for Amazon Reviews’, Stanford University.
[4] Wang, Q., Liu, P., Zhu, Z., Yin, H., Zhang, Q., and Zhang, L. (2019) ‘A Text Abstraction Summary Model Based on BERT Word Embedding and Reinforcement Learning’, Applied Sciences, vol. 9, no. 21, p. 4701.
[5] Nallapati, R., Zhou, B., Santos, C.N.d., Gulcehre, C. and Xiang, B. (2016) ‘Abstractive Text Summarization Using Sequence-to-Sequence RNNs and Beyond’, In proceedings of The SIGNLL Conference on Computational Natural Language Learning.
