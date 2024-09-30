---
layout: page
title: "Topics for Master Theses - Multilingual Grammatical Error Correction"
permalink: research/masters-topics-GEC/
author_profile: true
---

Hi! This is a small document talking about a possible topic for a master thesis.
If you find it interesting and want to work on this, don't hesitate to contact me!
If you are part of the masters in language technology (MLT) at Gothenburg University, you can select this topic with me and Elena Volodina as supervisors.
Arianna Masciolinni might also be available as co-supervisor (tbd depending on her schedule).

You can also find another topic [here](../masters-topics).

# Multilingual Grammatical Error Correction


## What is GEC?

The idea about GEC (grammatical error correction) is to offer language learners the possibility to correct their texts to a standardized version of the target language.
If you're thinking of something along the lines of [Grammarly](https://www.grammarly.com/grammar-check) you'll be on the right track.

Do note that despite the name of the task, not all of the corrections that we aim to make are grammatical in nature.
For example, we also care about lexical choices, syntax, and ortographic mistakes.

From the technical point of view, this task can be seen as some sort of translation task.
The source language is learner language while the target language being the corrected text.
Do note that there are some caveats with this, such as there being multiple possible corrections and whether fluency edits are valid or not.

A note about terminology: even though we talk about "corrections", the better term would be something along the lines of "correction hypothesis".
This is because the teachers must interpret the intent of the student and then determine what would be a better way to express it.


## The Multi-GEC data

This year we are launching a shared task for multilingual GEC.
The idea is to encourage people to develop technologies for languages other than English, particularly lesser-resourced languages.
Moreover, this allows us to compare how different languages behave in a GEC task.

You can find the main site for the Multi-GEC task [here](https://github.com/spraakbanken/multigec-2025).
If you're interested in it, we encourage you to participate on the shared task.
It will be part of the [NLP4CALL workshop](https://nlp4call.github.io/current/), which will be co-located with [NoDaLiDa/Baltic-HLT](https://www.nodalida-bhlt2025.eu/) next year in March.

Even though the project will be using the Multi-GEC data, it will be separate from the shared task.
This is partly due to the mismatch in timeframes but also it allows us to expand our scope even further than the original shared task.


## Ideas on what to work on

There are several ways in which we could take this project.
- The most simple one would be to develop systems that could have competed in the original shared task. That is, compare several types of models for the task and analyze their strengths and weaknesses.
- Another one could be to think of the metrics being used to evaluate these systems. At the moment we're offering GLEU, which requires a reference text, and the Scribendi score, which compares the proposed correction with a language model. Both of these metrics have their pros and cons. The idea here is to explore them and, if possible, to propose some improvements.
- A less technical approach would be qualitative evaluation. Designing good guidelines for human evaluation of these models can help shed light on things that automated scoring would not have caught. Moreover, it will also save time for human evaluators.
- There are two general filosophies when dealing with GEC. The first one is to do as few edits as possible. The second one is to also do correcitons for fluency. While both can be valid from a didactic standpoint, it is harder to prepare data for fluency corrections or to evaluate it. The idea here would be to compare approaches for both minimal and fluent approaches and to generate alternative training data for the fluency corrections.
- There is also a lot of research on [bias and fairness](../masters-topics) (another of the projects we're offering this year), but little of it has focused on the educational domanin. An intersection between the two projects could be to check how different language models perform, particularly those that claim to be multilingual. Once we find any discrepancies, we can attempt to reduce their impact.