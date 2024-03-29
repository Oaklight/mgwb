# Welcome to MANGO!

## What's MANGO?

**MANGO**: A Benchmark for Evaluating **Ma**pping and **N**avi**g**ati**o**n Abilities of Large Language Models

Large language models such as ChatGPT and GPT-4 have recently achieved astonishing performances on a variety of natural language processing tasks.
In this paper, we take an initiative to investigate their capacities of text-based mapping and navigation.
We propose MANGO, a benchmark that includes 53 mazes taken from a suite of textgames.
Each maze is paired with a walkthrough that visits all its locations but does \emph{not} cover all the paths.
The evaluation is zero-shot: for each maze, a large language model reads the walkthrough and answers hundreds of mapping and navigation questions such as "how should you go to Attic from West of House?" and "where are we if we go north and east from Cellar?".
It turns out that even the best to-date language model GPT-4 fails to give correct answers to a considerable portion of the questions, significantly underperforming humans. What's worse, GPT-4 works poorly on the challenging mazes that are larger and more complex.
Our benchmark can be used to track the advances of mapping and navigation abilities of large language models.
It will also facilitate future research that develops methods to improve such abilities of language models.
We host our data, source code, and evaluation programs at [https://mango.ttic.edu](https://mango.ttic.edu).

## Data location

TODO: links to different sections of Mango

## Cite Us

TODO: add bibtex
