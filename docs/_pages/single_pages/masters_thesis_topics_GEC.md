---
layout: page
title: "Topics for Master Theses - Multilingual Grammatical Error Correction"
permalink: research/masters-topics-GEC/
author_profile: true
---

Hi! This is a small document talking about a possible topic for a master thesis.
If you find it interesting and want to work on this, don't hesitate to contact me, Elena Volodina or Arianna Masciolini (`name.surname@gu.se`), all of whom are possible thesis supervisors.

You can also find another topic [here](../masters-topics).

# Multilingual Grammatical Error Correction

## What is GEC?

The idea about GEC (grammatical error correction) is to offer language learners the possibility to correct their texts to a standardized version of the target language.
If you're thinking of something along the lines of [Grammarly](https://www.grammarly.com/grammar-check) you'll be on the right track.

Do note that despite the name of the task, not all of the corrections that we aim to make are grammatical in nature.
For example, we also care about lexical choices, syntax, and ortographical mistakes.

From the technical point of view, this task can be seen as some sort of translation task.
The source language is learner language while the target language being the corrected text.
Do note that there are some caveats with this, such as there being multiple possible corrections and whether fluency edits are valid or not.

A note about terminology: even though we talk about "corrections", the better term would be something along the lines of "correction hypothesis".
This is because the teachers must interpret the intent of the student and then determine what would be a better way to express it.


## The MultiGEC dataset

This year we are launching a shared task for multilingual GEC.
The idea is to encourage people to develop technologies for languages other than English, particularly lesser-resourced languages.
Moreover, this allows us to compare how different languages behave in a GEC task.

You can find the main site for the MultiGEC-2025 shared task [here](https://spraakbanken.gu.se/en/compsla/multigec-2025).
If you're interested in it, we encourage you to participate.
Results will be presented on March 5th at the [NLP4CALL workshop](https://spraakbanken.gu.se/en/research/themes/icall/nlp4call-workshop-series/), which will be co-located with the [NoDaLiDa conference](https://www.nodalida-bhlt2025.eu/conference) in Estonia, Tallinn.

This means that, __even though you will be using MultiGEC data, you thesis project will be separate from the shared task itself, or at least from its competitive phase.__
This is partly due to the mismatch in timelines, but it also allows you to expand the scope of the project.

## Ideas on what to work on

There are several directions your project could take, and you are also welcome to propose your own idea.

- The most straightforward one would be to participate in the open phase of the shared task, i.e. to develop systems comparable to those submitted in the competitive phase.
- Another option could be to evaluate the metrics being used to evaluate these systems. At the moment we're offering GLEU, which requires a reference text, and the Scribendi score, which compares the proposed correction with the output of a language model. Both of these metrics have their pros and cons. The idea here is to explore them and, if possible, to propose alternatives.
- A less technical approach would be qualitative evaluation. Designing good guidelines for human evaluation of these models can help shed light on things that automated scoring would not have caught. Moreover, it will also save time for human evaluators.
- There are two general philosophies when dealing with GEC. The first one is to do as few edits as possible, with the goal of making the text acceptable from a purely grammatical standpoing. The second one is to also apply fluency edits. While both can be valid from a pedagogical standpoint, most MultiGEC corpora only have corrections in one of these two styles. You project could therefore focus on automatically generating additional training data for the languages that lack reference texts in one or the other style.
- There is also a lot of research on [bias and fairness](../masters-topics) (another of the projects we're offering this year), but little of it has focused on the educational domanin. An intersection between the two projects could be to check how different language models perform, particularly those that claim to be multilingual. Once we find any discrepancies, we can attempt to reduce their impact.
- Finally, if you want a software development challenge, your project could focus on building and testing a user-friendly application based on one or more of the submitted systems. From a research perspective, this would allow evaluating GEC systems on out-of-domain data, in the "real world".
