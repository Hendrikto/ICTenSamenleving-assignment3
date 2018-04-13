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

Where learning is defined as improving performance on a specific task without being explicitly told what to do. This improvement is achieved by looking at some kind of data. This does not exclude being taught, but only if it goes beyond explicit instructions like "if a then do b". [@10.1147] The definition also does not prevent having such rules as an outcome of learning, as long as the leaning entity comes up with them on its own.

Notice how we completely leave comprehension or understanding out of the picture here. Thus we also leave all the difficulties in defining what exactly that means behind us as well.

This definition is a lot narrower than the ones we looked at before, which is exactly its advantage: It does not leave important points open to interpretation. The rigidity of this definition allows us to draw an explicit line between intelligent and non-intelligent behavior. It also addresses the shortcomings of previous definitions as we will see.

## Application
According to our new definition, current so called "artificial intelligence" solutions are not in fact intelligent. As far as I can tell, there does not exists a system which can learn arbitrary tasks. There are a lot of ML systems around that are able to learn. However they are all limited to learning a specific task, which means that they are not intelligent.

If we apply the definition to "obviously intelligent" entities, like humans and many animals, such as dogs, we see that it matches our expectations. These entities are considered intelligent following the definition.

For humans this is obvious, as the whole education system with a myriad of different specialization options is a manifestation of this. Also every year new research areas are discovered. So far there has been no task humans were not able to approach by learning about it, even if it was previously unknown.

For another intelligent entity take dogs as an example. Dogs are able to learn every trick you can think of, as long as they are willing and physically able to do so. It may take them longer, and may need to be broken down into small steps compared to teaching the same to a person. This is why we consider dogs less intelligent compared to humans. In the end the dogs are able to learn though. Obviously not every dog is equally intelligent and equally motivated to use its intelligence, but this is not of importance here.

We can also use our definition to explain the situation where we had $a >_1 b$ and $a <_2 b$, so we could not decide whether $a > b$ or $a < b$. The problem with the tests is, that they do not actually measure intelligence, but its symptoms.

Typical "tests of mental ability" rank test subjects by asking them to solve a range of problems in some domains. [@gfactor] This is not an accurate measure of intelligence, as has been demonstrated before. There are totally non-intelligent systems which can score very well on these sorts of tests, based purely on statistical models. [@todai]

What these tests are actually measuring is how much you heave learned in some specific fields of study. They do not measure an entity's actual ability to learn. If you assume that each individual has the same motivation to use its intelligence by learning, and that they learn about the same things, then the score on these tests may be a good indicator for mental abilities. This is why in practice "people who do well on one kind of test tend to do well on the others, and people who do poorly generally do so across the board". [@gfactor] Still what we are measuring is not intelligence.

## Implications
The definition showcases that intelligence is an emergent phenomenon: If we succeed at implementing an ML system $x$ that is good at making ML systems, we can bootstrap an intelligent system. The ML system $x$ is not itself intelligent: It is able to learn generating ML systems, but nothing else. It does not generalize. The ML systems it generates are also specific and therefore not intelligent: They can learn one specific task which they were made for.

If we look at the whole AI consisting of $x$ and the ML systems $x$ can generate, intelligence emerges: If we ask the AI to learn an arbitrary task, $x$ can generate an ML system $y$ that is able to learn this tasks. If the AI has the ability to learn arbitrary tasks, which we have just demonstrated, it is intelligent according to our definition.

This is congruent with empirical evidence. The scientific consensus is that humans are intelligent (on the whole). We also know that the brain consists of a large amount of neurons, which are themselves not intelligent. [@10.1146] It obviously follows that at some point in between the neuron and the brain as a whole, intelligence emerges from non-intelligent subsystems. This conclusion is valid regardless of whether we know how this happens exactly. Indeed we currently do not know this, but luckily it must be true, so hopefully we will find out someday, by making use of our intelligence.
