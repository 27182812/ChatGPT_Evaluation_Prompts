# ChatGPT_Evaluation_Prompts
Collect ChatGPT prompts for NLG evaluation

## Prompt for ChatGPT to generate the prompts for each task
provide five concise prompts or templates that can make you deal with the [x] task

### Examples
provide five concise prompts or templates that can make you deal with the sentiment analysis task

Please give me three concise prompts for eliciting your ability to perform Aspect-Based Sentiment Analysis (i.e., extract the aspect terms and sentiment
polarity). There is no need to give examples, and do not limit the prompts to a specific product or domain.

## Prompts are based on one-to-five stars ranking
""" Score the following [task-ins] with respect to [aspect] with one to five stars, where one star means “[ant-aspect]” and five stars means “perfect [aspect]”. Note that [aspect] measures [aspect-ins].

[Conditioned Text]

[Generated Text]

Stars: """

where [task-ins] and [aspect-ins] are the instructions of the current task and aspect, respectively. [aspect] and [ant-aspect] denote the evaluated aspect and its antonym, respectively. [Conditioned Text] is the input of NLG models while [Generated Text] is theoutput.

### Examples
#### news summarization
Score the following *news summarization given the corresponding news* with respect to fluency with one to five stars, where one star means "*disfluency*"
and five stars means "*perfect fluency*". Note that *fluency* measures *the quality of individual sentences, are they well-written and grammatically correct. Consider the quality of individual sentences*.

News: [a news article]

Summary: [one generated summary]

Stars:



## Reference
[Is ChatGPT a Good NLG Evaluator? A Preliminary Study](https://arxiv.org/pdf/2303.04048.pdf)
