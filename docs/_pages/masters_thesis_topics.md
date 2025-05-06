---
layout: page
title: "Topics for Master Theses - Bias and Fairnes in AI"
permalink: research/masters-topics/
author_profile: true
---

Hi! This is a small document talking about a possible topic for a master thesis.
If you find it interesting and want to work on this, don't hesitate to contact me, Elena Volodina, or Simon Dobnik (`name.surname@gu.se`), all of whom are possible thesis supervisors.

The slides when presenting the topic in Autumn 2024 can be found [here](https://gist.github.com/rimusa/d92f6eaa18f06edbe91a05bb00027b04/raw/c96a181882d72e6f90afabf402ccc49715dcbad6/2025_Masters_Theses_Topic.pdf) and the video can be found [here](../documents/videos/masters_topic_presentation_2024.mp4).

You can also find another topic [here](../masters-topics-GEC).

# Bias and Fairness in NLP


## What do we mean by bias and fairness?

This past decade has seen AI applications being deployed at ever-increasing speeds.
These applications go from simple low-stakes tasks to life-changing high-stakes situations.
Some examples of AI-powered systems that have been deployed to high-stakes situations are: [medical systems assist medical practitioners](https://www.scientificamerican.com/article/health-care-ai-systems-are-biased/), [models that determine whether someone should get a loan or not](https://www.forbes.com/sites/korihale/2021/09/02/ai-bias-caused-80-of-black-mortgage-applicants-to-be-denied/), and [systems for law enforcement](https://www.technologyreview.com/2019/01/21/137783/algorithms-criminal-justice-ai/).

Ideally, we would expect that these systems don’t encode the same biases and prejudices that humans have.
However, machine learning approaches must look at human-generated data to learn and humans are indeed biased and prejudiced.
This leads to potential issues throughout the whole machine learning pipeline, from how we collect and aggregate the data to how we design and evaluate our models to how we implement these systems in the real world.
Given that deep learning tends to identify and exaggerate patterns in data, these biases have a very real potential of putting already disadvantaged groups even more at risk and of delaying the effects of social changes.

If you want to learn a bit more about these topics, I would recommend the following:
 - [Here's What Ethical AI Really Means](https://www.youtube.com/watch?v=AaU6tI2pb3M) is a video essay by Abigail Thorn from Philosophy Tube. It is a very good introduction to the whole topic of ethics in AI in a nice and entertaining format.
 - [Coded Bias](https://www.imdb.com/title/tt11394170/) follows Joy Buolamwini, one of the first researchers to tackle this problem. She explains how she first came across the issue of biases in AI and what she has noticed both in academia and on how it has been deployed in real-world situations. It's one hour and a half long, but it's an interesting watch.
 - There was [a tutorial at EMNLP in 2019](http://web.cs.ucla.edu/~kwchang/talks/emnlp19-fairnlp/) that explains bias and fariness both from a technological and from a human perspective. It is a bit dated on some of the technical stuff, but still interesting to look at. There was also [a tutorial at EACL in 2023](http://bit.ly/eacl23-ethics-slides) that I think is good but a bit harder to follow without the presenters as the slides have less text.
 - If you would like to look at papers in the topic, I can recommend the following two as a primer:
   - [Language (Technology) is Power: A Critical Survey of “Bias” in NLP](https://aclanthology.org/2020.acl-main.485) by Blodgett et al. is a very good introduction to the topic of unwanted biases and explains some of the pitfalls in which people tend to fall into when researching them. Section 5 is a case study and nicely illustrates these issues in the context of discrimination based on the use of African-American English.
   - [_A Framework for Understanding Sources of Harm throughout the Machine Learning Life Cycle_](https://dl.acm.org/doi/abs/10.1145/3465416.3483305) by Suresh and Guttag describes a framework to explain where biases might appear during the machine learning process and why they might appear. It has lots of examples and shows how a single source of unwanted bias can belong to more than one category.
   - If you've gone through these and would like to read a bit more, I have a longer list that I've been meaning to update and post somewhere. In the meantime, you can send me a message and I'll send you the list as it is at the moment.



## Where can we go from here

Even though this field encompasses all of AI, most of the research so far has focused in a small set of topics, namely:
 -	Most research on fairness and bias in NLP has (unsurprisingly) been done in English.
     -	The exception to this have been languages with grammatical gender that aligns with binary "semantic" gender (male/female), such as German and the romance languages.
     -	However, research on these other languages often focuses on the effects of grammatical vs semantic gender as opposed on the effects of biases themselves.
 -	When determining groups to check for bias, most papers tend to focus on:
     -	Gender as a binary (male/female)
     -	Race in the context of the United States, represented as a binary (black/white)

This means that there are a lot of possibilities on where we can expand upon, for example:
 -	Gender when taking into account identities other than male and female
     -	[Hannah Devinney](https://www.umu.se/en/staff/hannah-devinney/) works on the intersection between gender theory and NLP, see for instance [this paper](https://doi.org/10.1145/3531146.3534627).
 -	Biases against the LGBTQ+ community
     -	There is a dataset called [WinoQueer](https://aclanthology.org/2023.acl-long.507/) that is meant to check for biases in LLMs against the LGBTQ+ community.
 - In-group vs out-group biases
     - [This paper](https://aclanthology.org/2023.eacl-main.183/) analyzes how people from each party in the US talk about people in the other party in the Congress.
 - Biases based on names
     -	Names encode information about our culture and ethnicity, which can then reflect on the decisions that the model makes. There is much more work on this area than in others in this list, for instance [this one](https://aclanthology.org/N19-1424/). Still, I think there are interesting options that could be tackled here.
 -	Nationality/ethnicity/race
     -	These three concepts are heavilty intertwined but are [markedly distinct from each other](https://www.nationalgeographic.com/culture/article/race-ethnicity). Again, there have been many papers that tackle this issue ([this one](https://aclanthology.org/2023.eacl-main.9/) for example), but there are still options to explore. The idea is to avoid considering race as a binary task in this case. 
  

## Ideas on what to work on

There are several directions your project could take, and you are also welcome to propose your own idea.
 - Grammatical error correction (GEC)
   - "Hen" is a pronoun oficially introduced to Swedish [in 2015](https://svenska.se/saol/?id=1105387&pz=3) and is a gender-neutral way to refer to someone. However, due to lack of data it can be hard to work with it in some tasks, such as [POS tagging](https://umu.diva-portal.org/smash/get/diva2:1713349/FULLTEXT01.pdf). [Some work similar to this](https://aclanthology.org/2023.bea-1.13/) has been done for English.
   - There is also the [Multi-GEC data](../masters-topics-GEC), which is the other project we're offering this year. An intersection between the two projects could be to check how different language models perform, particularly those that claim to be multilingual. Once we find any discrepancies, we can attempt to reduce their impact.
 - Using [perspectivist ideas](http://pdai.info/) to tackle bias and fairness
   - Do systems become more fair if we create different models for each group?
   - How would these models interact with the test data for the other models?
   - Case study: automated essay grading with different models for different L1 profiles
 - Languages with more rich morphology
 - More to come in the following days... (bear with me while I deal with deadlines)
