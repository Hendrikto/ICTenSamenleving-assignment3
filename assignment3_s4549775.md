---
title: "Assignment 3: What does intelligence even mean?"
author: Hendrik Werner s4549775
date: \today
fontsize: 12pt
geometry: margin=5em
bibliography: bibliography.bib
---

# Introduction
In recent years the topics of machine learning (ML), artificial intelligence (AI), and their impact on society have become hot button issues. Specifically their influence on the job market is an often discussed issue, even though there are arguably more important aspects: Many leading researchers have long warned about the risks associated with AI [@ai_open_letter].

These discussions have often been overshadowed by an overarching problem: In most cases the concepts of machine learning, superintelligence, general intelligence, and artificial intelligence are thrown around without any clear definition of what intelligence means. A widely accepted definition is that intelligence is a measure of "overall mental ability" [@gfactor]. This does not really answer the question though, because it just shifts the question to: How do we define mental ability. Is there even such a thing as generic mental abilities, which is often called "general intelligence" [@gfactor]?

The goal of this article is to break down what intelligence means, and how it relates to current ML and AI research. Once we have established a solid definition, we can use it to properly talk about the (dis)advantages of some fields of research, the risks involved, and their societal influence.

The same problem which plagues privacy discussions also applies to intelligence: In the past, when talking about ML or AI, the discussions often failed because of diverging opinions on what intelligence is. If the participants don't agree on what the topic of their discussion is, it is very difficult to find common ground. Therefore the productivity of these discussion has not been as high as it could have been. We hope to rectify that with a better definition.

# Definition
## Prior work
Looking at the dictionary definitions of intelligence, we find multiple different versions:

* "The ability to acquire and apply knowledge and skills." [@oxford_intelligence]
* "the act of understanding" [@mw_intelligence]

  This is a very broad definition. What does understanding mean? If we look this up in the dictionary, it is defined circularly as "The ability to understand something" [@oxford_understanding]. And understand is defined as

  * "Perceive the intended meaning of (words, a language, or a speaker)" [@oxford_understand]
  * "Interpret or view (something) in a particular way" [@oxford_understand]

  None of this lets us really put a finger on what intelligence really means and does not help us draw a line between what is intelligent and what is not.
* "the ability to learn or understand or to deal with new or trying situations" [@mw_intelligence]

  This definition has the same problems as the one before with regards to "understanding" being ill-defined. It introduces further unclarities by referencing "new or trying situations". If an intelligent agent solved the trying new problem "1 + 1 = x", and then encounters the problem "1 + 2 = y", is that trying? Is that new? What about the problem "1 * 2 = x" (which can be broken down into "1 + 1 = x")?

  You could argue that all these problems are just applications of (repeated) addition, but you could also argue that each problem is new and trying. It is pretty obvious that this is not a rigorous definition, and still leaves much room for interpretation.
* "the ability to apply knowledge to manipulate one's environment or to think abstractly as measured by objective criteria (such as tests)" [@mw_intelligence]

  This definition also has multiple shortcomings, but let us address the most obvious one: If there is an objective criterion that can be measured with a test, then entities can be ordered by their intelligence based on their performance on this test. Now image the following situation: Entity $a$ scored better than entity $b$ on the first test: $a >_1 b$. Entity $b$ scored better in the second test than entity $a$: $a <_2 b$. This situation often happens in real world tests. Is is totally unclear whether $a$ or $b$ is the more intelligent entity.

  We assumed that there are objective criteria that can be a measure of one's intelligence. From this assumption we derived a contradiction. That means that the assumption must have been wrong. This is a classical proof by contradiction, which shows that the given definition has logical fallacies.

We can ignore the definition "the collection of information of military or political value" [@oxford_intelligence], which is not the type of intelligence ML and AI are dealing with.

As we have demonstrated, all the traditional definitions of intelligence are lacking if you want to have a scientific discussion based on them. In the following we want to establish a rigorous definition to enable founded, productive conversations on the topic.

## New definition
I propose the following definition for intelligence:

> The ability to learn arbitrary tasks.

Where learning is defined as improving performance on a specific task without being explicitly told what to do. This improvement is achieved by looking at some kind of data. This does not exclude being taught, but only if it goes beyond explicit instructions like "if a then do b". [@10.1147]

Notice how we completely leave comprehension or understanding out of the picture here. Thus we also leave all the difficulties in defining what exactly that means behind us as well.

This definition is a lot narrower than the ones we looked at before, which is exactly its advantage: It does not leave important points open to interpretation. The rigidity of this definition allows us to draw an explicit line between intelligent and non-intelligent behavior. It also addresses the shortcomings of previous definitions as we will see.
