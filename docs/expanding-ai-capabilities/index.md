# The Role of Databases in Modern Models

<!--more-->

Product owners like us exist at a fascinating juncture of technology and business. We are the fortunate soothsayers at the forefront of a revolution, witnessing artificial intelligence's gradual metamorphosis from sci-fi fantasy to reality. Yet, while we revel in the ongoing digital renaissance, it's impossible to ignore the hurdles that come with it. Let's embark on a brief journey through the current landscape of AI, focusing particularly on large language models (LLMs) and their workings.

AI today is a buzzing beehive of innovation. Everywhere we look, we see LLMs proving their mettle. From composing human-like texts and predicting stock market trends to assisting in medical diagnoses, these intelligent systems are making their presence felt. LLMs learn from vast amounts of data, absorbing patterns, nuances, and knowledge, a process akin to an enthusiastic learner in a gigantic library, reading and internalizing as much as they can.

LLMs operate on a simple principle. They're trained on enormous datasets, extracting valuable information and making sense of it through what we call tokens. Picture tokens as snippets of information, like pieces of a puzzle that the model assembles to gain understanding and provide responses. To make the most of an LLM, one needs to feed it as many tokens as it can handle, pushing the boundaries of its capacity to ensure comprehensive learning.

But here's the snag. We're constantly pushing the limits of the token count to equip the model with more knowledge, but doing so comes with its fair share of problems. There's a cap on the number of tokens these models can process effectively, and exceeding this token limit can lead to inaccuracies and 'hallucinations' where the model begins to generate content that doesn't align with reality.

More crucially, the conventional approach to training AI models is time-consuming and resource-intensive. The training process requires us to feed proprietary data into the system, which is not only a mammoth task but also raises concerns around data privacy and security.

So, are we resigned to these challenges, or is there a path that leads us towards a more efficient, accurate, and secure way of harnessing the power of LLMs? I believe there is, and it involves a fundamental shift in our approach, swapping the model training with a mechanism that allows AI to interact with databases directly.

As we venture further, we'll unpack this new approach, exploring its potential benefits and implications, and why I think it's a game-changer in the realm of AI.

![Image](/images/expanding-ai-capabilities-2.png)

 To fully appreciate the transformative potential of the new approach I'm advocating for, it's necessary to delve a little deeper into the issues faced with the conventional methods of training AI models.

Our current approach to machine learning models hinges heavily on training. We teach models to learn and reason by exposing them to vast volumes of data, allowing them to understand patterns, context, and relationships. This training phase is crucial, determining the model's eventual accuracy and its ability to handle complex tasks.

However, the size of the training data and the time and computational power required for effective learning can make this process a formidable undertaking. Besides, the need to constantly update the training data to ensure the model remains relevant adds to the complexity. There's also the question of the proprietary nature of data and the stringent need to adhere to data privacy norms.

Then, we have the token limit problem, the invisible boundary that prevents us from stuffing our models with as much knowledge as we'd like. Each token a model processes eats into its total capacity, and exceeding this limit can lead to a degradation in the quality of the model's responses.

With these challenges at hand, what if we could pivot to a different strategy? One where we don't have to worry about the token limit or go through the painstaking process of training the model on proprietary data? I propose a way where we can use off-the-shelf AI models, pair them with a database containing our proprietary data, and instruct these models on how to interact with this data using SQL commands.

Imagine the possibilities. The model wouldn't have to consume tokens to learn from the data because it would have direct access to the database. It wouldn't need to be trained on proprietary data because it would generate SQL commands to interact with the data when needed. We would essentially have a dynamic AI model, capable of pulling data and learning on the go.

This approach isn't about dismissing the importance of training AI models. Instead, it’s about exploring a complementary path, one that promises efficiency, flexibility, and an enhanced level of accuracy. In the next section, we'll dive deeper into how this new approach works, its mechanics, and its potential benefits. 

![Image](/images/expanding-ai-capabilities-3.png)

 So how exactly does this new approach work, and why should we, as product managers, pay attention to it?

Here's the thing. When we interact with databases, we don't dump all our information into a query and expect a useful response. Instead, we use SQL commands to define our requests precisely, so the database understands and retrieves what we need. In the same way, we can use off-the-shelf AI models and teach them to interact with databases via SQL commands.

Think of it this way: we're giving our AI model a map and a dictionary. The map is the structure of the database, and the dictionary is the set of SQL commands. By knowing the structure and how to manipulate it using SQL, the model doesn't have to remember every piece of data - it can simply query for it when needed. This reduces the load on the model, since it doesn't have to hold all the tokens in memory, and eliminates the risk of exceeding the token limit.

But how does it process queries? Let's break it down. When a query comes in, instead of throwing the model into the deep end, we ask the model what SQL commands it should perform first. The model, having been taught to interact with the database, will issue SQL commands based on the query. We then provide the model with the results of these commands. Now that the model has specific, relevant data to work with, it can process the query and provide a response, without hallucinating or struggling to connect dots from an overflow of tokens.

In essence, we're simplifying the process and making it more efficient. The model no longer needs to be fed with proprietary data or pushed to its token limit. It can use its symbolic memory, the SQL database, to access and manipulate data as needed.

This approach is not just about creating a faster, leaner AI model. It's about re-imagining the way we view AI capabilities. It's about leveraging the power of existing tools, like SQL databases, and finding ways to make them work in harmony with AI models.

![Image](/images/expanding-ai-capabilities-4.png)

 Now that we have a better understanding of this new approach, let's talk about why it’s worth our attention. Why should we, as product owners, care about this shift, and what potential benefits does it bring to the table?

Firstly, efficiency. With this approach, our AI models no longer have to shoulder the entire load of processing vast amounts of proprietary data. By teaching them to interact with databases via SQL commands, we simplify the process, reducing the demand on computational resources and enabling a more streamlined approach to handling queries.

Secondly, this approach addresses the token limit issue head-on. By allowing the model to directly access the data it needs to process a query, we eliminate the need to overload the model with tokens. This not only prevents the risk of 'hallucinations' but also improves the accuracy of the model's responses.

Next, we have the matter of data privacy. When we train models using proprietary data, there's always a risk, however minute, of sensitive information being inadvertently leaked. By allowing the model to interact directly with a secure database, we can better protect proprietary information while still giving the model access to the data it needs.

But, the advantages go beyond just improving efficiency and preserving data privacy. I believe this approach could open the door to more dynamic, adaptable AI models. By having direct access to databases, AI models can stay up-to-date with the latest data without needing to go through a new round of training each time there's an update. This adaptability is a game-changer in industries where real-time data is crucial.

Finally, this new approach offers an exciting prospect: the ability to leverage AI models in new ways without needing to retrain them on new data. Instead of creating a model for every new project, we could utilize off-the-shelf models in diverse applications, saving both time and resources.

Make no mistake, this isn't a magic wand that will solve all the complexities of AI overnight. But it represents a promising step towards a more efficient, accurate, and secure way of leveraging AI.

![Image](/images/expanding-ai-capabilities-5.png)

 Given the benefits and potential of this new approach, it's easy to envision its applicability across a wide array of domains. However, let's zoom in on a single, highly relevant application for most businesses today: customer support.

Imagine a scenario where an AI model assists a customer support agent during a call. In this scenario, the AI model has access to a database that contains information about all the capabilities the agent can offer, as well as data related to the customer's history, preferences, and previous interactions. As the conversation unfolds, the agent receives real-time suggestions from the AI model on the best next action to take or the most suitable solutions to offer, based on the live dialogue and the historical data pulled from the database.

This could transform the way customer service is delivered. Instead of requiring the agent to remember every policy, procedure, and product detail, they would have a smart assistant offering contextually relevant advice. This would not only speed up the call resolution time but also significantly improve the quality of the service delivered. It would be a more efficient, accurate, and personalized approach to customer support.

After understanding the potential this new approach holds for customer support, one can extrapolate its benefits to other fields. In healthcare, an AI system could interact with databases of medical conditions, symptoms, and treatments to assist doctors. Financial institutions could leverage AI models to interact with databases of market data and economic indicators to provide real-time insights.

Naturally, this approach isn't without challenges, such as ensuring database security, dealing with potential bias in the AI's SQL command generation, and making sure the AI understands the database structure correctly. But every challenge presents an opportunity for us to innovate, learn, and grow.

This vision of AI actively participating in the data dialogue, and not just passively consuming tokens, brings us closer to a future where AI is more efficient, accurate, versatile, and seamlessly integrated into our digital ecosystems.

As we stand on the cusp of this exciting new era, it's clear that our journey with AI is far from over. It’s merely evolving, opening up new pathways to explore and new vistas to conquer.

----
Note: This was first published as a [LinkedIn article](https://www.linkedin.com/pulse/expanding-ai-capabilities-role-databases-modern-erik-gaius-capistrano/?trackingId=MBw6%2Fm2GS2o8Tr8BDBGB6g%3D%3D).
