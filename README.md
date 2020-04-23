# Pipeline
![Pipeline](https://github.com/DmitriyValetov/nlp_course_project/blob/master/pipeline.png)

# Q&A
a) What is the problem you are trying to solve? Why is it important? 

Main objective is to improve the quality of text summarization by using the topic (aspect) of the text. 
Our task is to hybridize topic modelling and summarization. 
Particularly - to use aspects vectors in the summary generation process. And therefore manipulate the focus of the summary.
Subtask is to check whether an aspect can influence the result of summing text  E.g. generate a different summary of the text by bias to one or more of its topics: text about sport event with attention to politics, should (from our point of view) summarize more information about famous people who attended the event, than about the event itself.

b) What are the existing solutions for this problem? If the problem is new, describe the solutions of the most relevant problems to yours.

Topic extraction:
1. Attention Based Aspect Extraction https://www.aclweb.org/anthology/P17-1036.pdf https://github.com/ruidan/Unsupervised-Aspect-Extraction https://github.com/madrugado/Attention-Based-Aspect-Extraction 
2. LDA (Many)
3. Zhao, Wayne Xin, et al. "Jointly modeling aspects and opinions with a MaxEnt-LDA hybrid." Proceedings of the 2010 conference on empirical methods in natural language processing. Association for Computational Linguistics, 2010.
4. ARTM Vorontsov, Konstantin, and Anna Potapenko. "Additive regularization of topic models." Machine Learning 101.1-3 (2015): 303-323.https://link.springer.com/article/10.1007/s10994-014-5476-6 https://bigartm.readthedocs.io/en/stable/index.html
5. BTM Xiaohui Yan, Jiafeng Guo, Yanyan Lan, and Xueqi Cheng. 2013. A biterm topic model for short texts. In Proceedings of the 22nd International World Wide Web Conference. 
6. SAS Zhiyuan Chen, Arjun Mukherjee, and Bing Liu. 2014. Aspect extraction with automated prior knowledge learning. In Proceedings of the 52nd Annual Meeting of the Association for Computational Linguistics.
7. k-means

Summary generation:
1. bart / pegasus / electra https://arxiv.org/pdf/1901.07786.pdf
2. Bert https://paperswithcode.com/paper/text-summarization-with-pretrained-encoders
3. With fixed size  https://paperswithcode.com/paper/positional-encoding-to-control-output 
4. PEGASUS: Pre-training with Extracted Gap-sentences for Abstractive Summarization: https://arxiv.org/pdf/1912.08777.pdf 
5. SummaRuNNer: A Recurrent Neural Network based Sequence Model forExtractive Summarization of Documents: https://arxiv.org/pdf/1611.04230.pdf 
6. Sample Efficient Text Summarization Using a Single Pre-TrainedTransformer: https://arxiv.org/pdf/1905.08836.pdf 
7. Language Models are Unsupervised Multitask Learners: https://d4mucfpksywv.cloudfront.net/better-language-models/language-models.pdf 
8. Neural Text Summarization: A Critical Evaluation: https://www.aclweb.org/anthology/D19-1051.pdf 
9. Exploring the Limits of Transfer Learning with aUnified Text-to-Text Transformer: https://arxiv.org/pdf/1910.10683.pdf 
10. MASS: Masked Sequence to Sequence Pre-training for Language Generation: https://arxiv.org/pdf/1905.02450.pdf 
11. Multi-News: a Large-Scale Multi-Document SummarizationDataset and Abstractive Hierarchical Model: https://arxiv.org/pdf/1906.01749.pdf 
12. A Discourse-Aware Attention Model forAbstractive Summarization of Long Documents: https://arxiv.org/pdf/1804.05685.pdf 
13. Don't Give Me the Details, Just the Summary! Topic-Aware Convolutional Neural Networks for Extreme Summarization: https://arxiv.org/pdf/1808.08745.pdf 
14. Teaching Machines to Read and Comprehend: https://arxiv.org/pdf/1506.03340.pdf 
15. Attention Is All You Need: https://arxiv.org/abs/1706.03762 
16. Alexander M. Rush, Sumit Chopra, and Jason Weston. 2015. A neural attention model for sentence summarization. In Proceedings of the 2015 Conference on Empirical Methods in Natural Language Processing. http://www.emnlp2015.org/proceedings/EMNLP/pdf/EMNLP044.pdf

c) What is the data you will be working with? Is it an already released dataset? If so, please provide a description and a link to it. If it is a new one, please describe your methodology to collect the dataset.

1. Dataset RossiyaSegodnya https://github.com/RossiyaSegodnya/ria_news_dataset 

d) What is your team? If there is more than one person, please provide provision responsibilities for all people. 

![Task weights](https://github.com/DmitriyValetov/nlp_course_project/blob/master/work.png)

e) How are you going to solve the described problem? What are the differences from the baselines you are comparing with? Please do include a link to a repository where you are going to keep the solution's code and data in case you are collecting  the dataset.
1. Topic/aspect extraction. 
2. Summarization with extracted topics/aspects.
