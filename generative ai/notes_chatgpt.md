# [Complete AI Guide: Chat GPT, Midjourney, Dall-E 2, Generative AI, Prompt Engineering](https://www.udemy.com/course/complete-ai-guide/learn/lecture/36484970#content)


## [x] Intro  6m
## [wip] Fundamentals + Chat GPT Prompt Ideas   39m

> What is chatGPT?
    AI language model trained on text data generating converationally natural language responses

  **chat gpt is a conversational tool that can help find the right questions to ask while synthesizing large amounts of specifically tailored information**

> Benefits
    - Saves Time
    - Extend Reach Beyond Field of Expertise

> Outputs
    - Synthesize: process large amounts of content concisely
    - Content & Copy Creation: generate new content for specific topic and purpose
    - Learn & Research
    - Coding



[ChatGPT:](https://chat.openai.com/auth/login)

> Purpose : 
    interactive tool to intelligently and iteratively process queries with responses that are personalized to user specs & prompts

> Input/Output : 
    queries occur in a conversational-style succession of questiosn to iterate and refine the ai's output
    
> Scope : 
    limited to the data the model's been trained on


[OpenAI Playground](https://platform.openai.com/playground)
    
    the playground provides additional parameters, presets, layouts and fine grained control to effect our output

some addtl functionality in the playground
> [insert]
> remove [insert]
> fix grammar // more specifically
> comprehension level dropdown
> speech to text

[OpenAI's security and privacy](https://openai.com/security)
[OpenAI's blog post on recent updates](https://openai.com/blog)
[OpenAI's focus on user and AI safety](https://openai.com/safety)


<br>
<hr>
<br>

### **Creating EFFECTIVE Prompts**

*Consider Levels of Explanations, Broad vs Narrow*

> explain xyz as... a 1st grader, grad student, leading expert
> top xyz  vs  top xyz for a beginner

<br>

*Consider the context of your prompt*
... define how you want chat gpt to engage with you

> you're going to act as...
> ignore all previous instructions
> respond with a friendly and casual tone
> respond with a serious and formal tone
> explain this to a 5 yr old
> you're an exercise and health expert. you've helped all ages of people


*Give your model a task to complete*
... aka compression vs decompression
> your task is to describe XYZ in XYZ words."     

*Be specific* 
> "do not include XYZ, remove this symbol/number."

*Ask questions*
...Further elaborate on specific outputs from the previous answer. 

> breakdown answer #5 of this list
> I don't like how the bridge sounds, can we change that to be more xyz..


*Consider the output* 
    
    If you don’t like your results, refine your prompt to be as specific as possible 
    aka => 
        gold in == gold output
        garbage in == garbage output

    You have to work WITH chatGPT to get the output that you want

https://github.com/f/awesome-chatgpt-prompts
https://github.com/f/awesome-chatgpt-prompts/blob/main/prompts.csv


*Modifiers & Prompt Ideas to Better Iterate on your Outputs*

    The choice of modifier you use will greatly impact the quality of your outputs

> Qualifiers
> Adjectives
> Adverbs
> Intensifiers
> Negatives
> Number words
> Time words
> Place words
> Degree words

> What would I not think of on this topic?
> What are some uncommon or lesser used approaches to this problem?
> Give me something original around this topic that some people believe to be untrue


<br>
<hr>
<br>

### Tokens
    - tokens represent chunks of data bits in the conversation
    - token limits noted are aggregates for both inputs and outputs
      - (mindmap limits as RAM capacity)
    - as the convesation approaches the token limit=> 
      responses can become: 
        - less accurate
        - less reliable
        - a bit more non-sensical
    - longer conversations exceeding the token limit will...
        - begin forgetting the beginning of the conversation to maintain token limit
        - subsequent responses will not encompass 'forgotten' information

GPT4 has an *8000 token limit*
GPT3 has an *3096 token limit*

|------------------------------------
|  *approximate conversions ratios* |
|                                   |
|  1 token == 4 chars == .75 words  |
|  100 tokens == 75 words           |
|  30 tokens == 1-2 sentences       |
|  100 tokens == 1 paragraph        |
|  2048 tokens == 1500 words        |
|------------------------------------

   *working around the token limit*
> prompt for a summary of the conversation to that point
> copy and paste into a new convo or just continue in the same conversation
> the summary will retain the relevent points to maintain context for the model and conversation

[estimate a token count](https://platform.openai.com/tokenizer)


<br>
<hr>
<br>

## [] Prompt Engineering & Prompting Guide   66m
<hr>

## a specific limitation to note
> current cutoff date for chat gpt training data is 09/2021

    this means that responses are only 'accurate' to that date ->
    i.e.
    - chatgpt is NOT an online search tool like google
    - static information like the laws of thermodynamics or pythagorean theorem WILL be correct
    - newer data like financial or sporting statistics from 2023 or the latest version of React will NOT be included in response synthesis

**to incorporate data that the AI was NOT trained on...**
> <prompt_priming> => inject / copy and paste the data or links to data into the conversation
> browser extensions exist 


## your output is only as good as the data the model was trained on...

**... and the prompts the user provides**

> the better the prompt, the better the output


> [] create prompt templates!


## Prompt Engineering
<see guide for more details>
- good prompt criteria
- main prompting steps
- prompt priming
- simple prompt starters
- prompt revisions


## Prompt Frameworks
<see guide for examples and more details>

> Shot Prompting: injecting prompt w/ params and ref data (aka shots)
    - types: [zero, one, multi-shot]
    formula: 'using xyz as reference ...'

> Chain of Thought Prompting: model explains answers step by step
    formula: 'let's think step by step'

> Tabular Format Prompting: creating tables
    formula: 
        - query
        - 'what diff categories can your answer can be broken down to for more descriptiveness'
        - 'create a table including the original answer separated into diff columns per those categories'


> Ask Before Answer Prompting: guide model to ask for clarifications before giving an answer, adding accuracy and specificity
    formula: 
        - 'you are..... but before you answer, I want you to ask  questions about..."
        - 'please ask any questions you have so that i can improve my prompt before you complete your task'

> Fill in the Blank Prompting: encourages deeper thought processes, learning and communication
    formula:
        - <see guide>

> Perspective Prompting: broaden your understanding with a comprehensive view of a topic for more informed decisions and nuanced understanding of complex topics

> Constructive Critic Prompting: provide objective and expert feedback, highlight areas for improvement and offer constructive criticism

> Comparative Prompting: highlight key similarities and diffs for more informed decisions and deeper understanding of strengths, weaknesses and tradeoffs

> Reverse Prompting: reverse engineer content

*these establish a standardized format to optimize framign and performance*
> RGC Prompting
> I Want You To Act As Prompting


## [] Simplify Complexity, Proofread & Reorganize Data   31m


## [] Content Creation, Social Media, Copywriting, SEO, & Video Scripts    50m
## [] Learn, Research and Prepare    60m
## [] Use Cases, Spreadsheets, and Training GPT    17m
## [] 
## []
## []
## []
## []
## []
## []



