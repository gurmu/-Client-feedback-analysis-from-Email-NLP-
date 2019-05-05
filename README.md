# -Client-feedback-analysis-from-Email-NLP-
NLP is the ability of machines to understand and analyze human language. It is a part of the Artificial Intelligence (AI) domain with a significant overlap with Linguistics.
However, natural languages are extremely complex systems. Think of a human body; it consists of 11 separate systems (e.g., nervous, digestive etc.) working in tandem with each other. Similarly, a human language has several sub-systems such as phonology, morphology, and semantics working seamlessly with each other.

This complex interplay of different sub-systems makes learning a new language a difficult proposition. If you are a native English speaker it will probably take you 2,000+ class hours to be fluent in Mandarin. That’s several years’ worth of studying! This is the reason why the progress in NLP has been slow as compared with other areas within Machine Learning and AI.
NLP Process Flow:
A typical NLP process flow has the following steps:
1) Data Collection: Data mining or ETL (extract-transform-load) process to collect a corpus of unstructured data.

2) Data Preprocessing:

Tokenization: Segmentation of running text into words.
Lemmatization: Removal of inflectional endings to return the base form.
Parts-of-speech tagging: Identification of words as nouns, verbs, adjectives etc.
3) Feature Engineering:

Word Embeddings: Transforming text into a meaningful vector or array of numbers.
N-grams : An unigram is a set of individual words within a document; bi-gram is a set of 2 adjacent words within a document.
TF-IDF values: Term-Frequency-Inverse-Document-Frequency is a numerical statistic representing how important a word is to a document within a collection of documents.

4) Application of NLP Algorithms:

Latent Dirichlet Allocation: Topic modeling algorithm for detecting abstract themes from a collection of documents.
Support Vector Machine: Classification algorithm for detection of underlying consumer sentiment.
Long Short-Term Memory Network: Type of recurrent neural networks for machine translation used in Google Translate.
Now let’s look at a couple of real-life case studies on actual customer complaints.
Case Study #1: Topic Modeling
Problem: While filing a complaint, customers are asked to choose the complaint category or theme. However, customers are unaware of business terms so they often choose the wrong category. This was a major issue for us with more than 20% of complaints being misclassified and routed incorrectly. This led to long wait times and incomplete resolution of customer complaints.

Solution: We leveraged topic algorithms such as TF-IDF and LDA to reclassify customer complaints based on the exact language used in the complaint. As seen in the chart below, there are several differences between original (customer-led) and new (NLP-recommended) themes. Especially, NLP-themes identified ‘Late Fees’ as the main reason (17%) for customer complaints, which was considerably higher than the previous estimate.

This analysis identified the root cause of complaints much quicker and with more precision. Despite this breakthrough, we were still struggling to categorize complaints with 100% accuracy. Sometimes a single complaint had multiple aspects that could be attributed to several categories and this led to inaccurate categorization and improper resolution efforts. To improve accuracy, we built a customized knowledge graph or network map of all complaints using cosine similarity metric which acted as gravitational force between individual complaints. Moreover, force-directed graphs were leveraged for better visualization.

I know what you are thinking! Yes, it does look like a weird sea coral! But every node in this knowledge graph is an individual complaint. Similar complaints are clustered together based on the exact language used and represented by different colors. Using this analysis, we were able to glean the following insights:

Multiple Complaint Themes: A typical complaint has 2 or 3 different themes. Representation of complaints through knowledge graphs allows for better identification of overlapping themes and outliers within a cluster.
Central vs. Peripheral Themes: In the above graph, ‘Account Closures’ is a central topic and improving closure experience can benefit other themes. In contrast, ‘Social Security’ complaints live on their own island and hence they need to be approached with a separate resolution strategy.
Hidden Themes: Knowledge graphs can uncover hidden relationships in the unstructured data and help identify new themes.
Results: Based on these insights, we determined that ‘Customer Fees’ was a much bigger issue than previously believed. We eliminated foreign transaction fees for approximately 1.5 million customers. We also revamped our late fee policies, implemented more customer-centric standards, and waived late fees for approximately 30 thousand customers a year. These efforts ultimately led to our highest-ever customer satisfaction score and lowest complaint rate in the last 4 years.

Case Study #2: Sentiment Analysis
Problem: Historically, we were oblivious to underlying sentiments in customer complaints. Obviously, complaints are all about negative customer experience but it is important to find out whether customers are questioning a policy or if they had a truly dreadful experience that should have been avoided at first place. Essentially, we needed to quantify the customer ‘piss off’ factor to prioritize and escalate complaints that needed to be handled right away.

Solution: For sentiment analysis, we maintained a standard NLP workflow with a few additional key steps. Firstly, there was a sentiment detection step where a bag-of-words model was leveraged to determine whether the text pertains to an objective fact or opinion through lexicon-based approaches. Secondly, the polarity of sentiment (positive or negative) was determined through Machine Learning algorithms. We tested several classification algorithms including Random Forest, Support Vector Machines and Gradient Boosting. Deep Learning algorithms, especially Long-Short-Term-Memory (LSTM) networks which have the ability to forget irrelevant information also showed a lot of promise. Once consumer sentiments were aggregated, they were mapped back to the knowledge graphs for better visualization.
As you can see, the ‘Fraud and Identity Theft’ theme was associated with the most negative consumer sentiment. Other problematic complaint themes were ‘Merchant Disputes’ and ‘Credit Line Decrease’. In addition, customer sentiments were tracked over time by developing a sentiment dashboard. This was done mainly because business executives love dashboards! An example is included below.
Results: This analysis led to a comprehensive review and subsequent improvement of our fraud prevention program and better merchant dispute/credit practices. Importantly, taking these steps towards enhancing our customer advocacy initiatives, elevated us from 7th position to 3rd position in 2018 J.D. Power Satisfaction study.
