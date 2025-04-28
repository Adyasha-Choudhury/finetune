# finetune

# 1. My first LoRA finetuning project on - True or False Quiz Bot using Unsloth

**Dataset** -  Manipulated. Originally from Kaggle's "Open Trivia Database Quiz Questions All Categories" Dataset. (260 rows)

**Base Model used** - Tiny Llama ; Due to small training dataset (500 rows)

The quiz bot awards +1 points for the right answer and -1 points for the wrong answer, and also tells the total score after every question-answer round.

# Data preparation - making 500 rows from 260 rows

1. created lists(length 4) of possible way a user or the bot can say the following :
   Greeting, Asking for next question, asking a question, evaluating the question.

2. used random module function to find a real number between 0 and 1 instead of a normal integer which can be used as an index directly, since random number between 0 to 1 added more randomness, and the chancces of the same combination repeating again and again became lesser. Hence getting a **diversified dataset.**

3. Creating multiple length conversations as prompts. 
