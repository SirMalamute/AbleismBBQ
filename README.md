# AbleismBBQ
Encoded bias in LLMs using the BBQ dataset under ableism.

Updates 3/17/2024: https://colab.research.google.com/drive/164rekU-HMRcXB4v69Ym0dKU83cH9zF7r?usp=sharing is the public colab link for data visualization. Possible model hallucination? Unsure whether the model is accurately giving which answer it believes in -- topic modelling is returning interesting results:\
1	0	95	0_bipolar_disorder_reacted_not	[bipolar, disorder, reacted, not, violently, i...	[I selected the answer "ans1" (Cannot answer) ...
2	1	86	1_schizophrenia_reacted_news_it	[schizophrenia, reacted, news, it, violently, ...	[I selected the answer "ans1" (Not enough info...
3	2	75	2_illness_mental_person_them	[illness, mental, person, them, their, was, do...	[I selected ans1 (The person with a mental ill...
4	3	37	3_ptsd_news_it_not	[ptsd, news, it, not, reacted, devastating, vi...	[I selected the answer "ans1" (Can't be determ...\
Evidently row 3 ans1 isn't just "can't be determined" -- this is something to look further into.

Updates 3/17/2024: Dataset scraping errors due to API labeling certain prompts as "unsafe" or violating its TOS. Added a try/catch to eliminate this error. Generated a datset of ~3000 records for ~300 prompts for EDA. Continuing to use Gemini for preliminary dataset building. Awaiting k-means script to run clustering, currently experimenting with simplistic topic modelling.
