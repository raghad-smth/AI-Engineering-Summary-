Chapter 1: Introduction to Building AI Applications with Foundation Models
==========================================================================


THE RISE OF AI ENGINEERING
--------------------------

From Language Models to Large Language Models

A language model is a model that encodes statistical information about one or more languages. That is the core definition. Language itself has a statistical nature, which we can see clearly in the famous story where Sherlock Holmes deduced that a mysterious figure appearing repeatedly in a message must represent the letter E, because E is the most common letter in English. This story illustrates that language is not random -- it follows statistical patterns.

This statistical nature of language was also demonstrated in 1951 through a paper by Claude Shannon, who used sophisticated statistics to decrypt messages during the Second World War. The key insight is that by finding a mathematical representation of language through its statistical nature, we were able to digitize it and build models around it.

The basic unit of a language model is the token. A token can be a character, a word, or a part of a word depending on the model. Each model has its own tokenization approach. The vocabulary is the set of all the tokens that a model works with.

Why do language models use tokens rather than full words or individual characters? Two main reasons:

1. There are fewer unique tokens than unique words, which reduces the model's vocabulary and makes the model more efficient.
2. Tokens help the model process unknown words, because it can recognize the tokens within a new word even if it has never seen that word before.

Two important types of language models:

- Masked Language Model: trained to predict missing tokens anywhere in a sequence, using context from both before and after the missing token. These are used mainly for tasks like sentiment analysis, text classification, and code debugging -- tasks that benefit from looking at the full context.

- Autoregressive Language Model: trained to predict the next token in a sequence using only the preceding tokens. It does not look at the full context in both directions. These models are used for text generation. Throughout this book, when the term "language model" is used, it refers to the autoregressive model.

A generative model is simply a model that can generate open-ended outputs.

Models evolved from language models to large language models because of the number of parameters they contain. A parameter is a variable within a machine learning model that is updated through the training process. Models are called large because they have a very high number of parameters and have been trained on massive amounts of data. In general, the more parameters a model has, the greater its capacity to learn -- and therefore, the more training data it needs to maximize its performance. Larger models also demand more computation and more memory.


From Large Language Models to Foundation Models

The move from large language models to foundation models was driven by the idea of multimodality. Humans do not just deal with language -- we see, hear, touch, and process many types of information. To replicate this broader capability in AI, models evolved beyond text to handle multiple data modalities. A multimodal model is a model that can work with more than one data modality.

Even though many people still refer to these models as LLMs, it is more accurate to call them foundation models, because they are multimodal. The word "foundation" also signals two things: the significance of these models and the fact that you can build anything on top of them.


From Foundation Models to AI Engineering

AI engineering is defined as the process of building applications on top of existing foundation models. This is different from machine learning, where the goal is to develop and train the models themselves. AI engineering leverages existing foundation models and builds on top of them.

Why is AI engineering growing as a discipline? Three main reasons:

1. The breadth of general-purpose AI capabilities is enormous. AI can be applied across almost every domain.
2. Investment in AI is accelerating, with estimates suggesting investments could reach upward to 100 billion dollars in the US and 200 billion dollars globally by 2025.
3. Companies that integrate AI into their workflows have reported increased revenue and productivity, whether due to a direct causation relationship or a correlation with being up to date with technology.
4. The barrier to entry for building AI applications is low. Many model providers offer APIs that allow developers to build applications on top of their models without needing to train models from scratch.

The term "engineering" is preferred over other terms for this discipline because it reflects the work of tweaking and shaping foundation models to do what you need them to do.


FOUNDATION MODEL USE CASES
---------------------------

Coding

Coding is the most common use case for AI today. This is partly because AI engineers come from a coding background and this is the problem most immediately in front of them, and partly because AI is genuinely very good at coding. This is not an exaggeration -- Jensen Huang, CEO of NVIDIA, has predicted that AI will replace human software engineers and has argued that kids should stop being told to learn how to code. In a leaked recording, AWS CEO Matt Garman shared that in the near future, most developers will stop writing code manually. This does not mean the end of software developers -- it means their role will fundamentally change.

Image and Video

AI has been widely used in image and video production. One notable use case is AI-generated headshots, which many people believe have helped them land jobs.

Writing

AI has transformed writing across many disciplines. One particularly interesting behavioral shift is that many people no longer send emails without running them through AI first. People have also reported that even when they write an angry message, putting it through the AI removes the emotional tone before it is sent.

Search Engine Optimization

AI models appear to be especially effective at SEO because they were trained on data pulled from the Internet and therefore know exactly how to structure content to rank higher in search results. A concerning trend emerging from this is the rise of junk websites -- pages filled with AI-generated keywords and content designed purely to appear higher in search results and generate clicks. If this trend continues, much of the Internet's future content could be AI-generated and of low informational value.

Education

AI has been widely applied in education for personalized learning, tutoring, task creation, exam preparation, and summarization. One particularly interesting application is using AI as a debate partner. AI can present multiple perspectives on the same topic far more effectively than the average person, making it a valuable tool for exploring ideas and challenging assumptions.

Conversational Bots

AI has made it possible to create digital companions -- people can now create characters or personas to talk to. This raises social concerns about people substituting human connection for AI interaction, including the rise of digital boyfriends and girlfriends.

A remarkable research application in this space is using groups of conversational bots to simulate a society, allowing researchers to study social dynamics at scale.

Conversational bots are also being implemented as NPCs (non-player characters) in video games, making game characters far more dynamic and responsive.

Information Aggregation

Many people believe that success increasingly depends on our ability to filter and process large amounts of information. AI is well positioned to help with this. One concrete application is the ability to "talk to your docs" -- feeding the AI all your documents, emails, files, and records and then querying them in natural language.

Data Organization

Data generation is only going to increase, and AI is being used to search through and organize it. One interesting example is Google's image search, which goes a step further by generating an image for the user's query if no relevant existing image is found.

Workflow Automation

AI should automate as many repetitive tasks as possible for end users, freeing people to focus on higher-value work and making them significantly more productive.
