# Assignment 3 - Write UP

## Description
This assignment completes our movie chatbot system by implementing action functions that query our movie database and building a natural language interface. You implemented functions to search for movies by year, director, and actors, as well as the core search system that matches user queries to appropriate database operations. This builds directly on the pattern matching work from Assignment 2 to create a functional conversational AI system.

## What to complete
1. Complete all action functions in `a3.py` (title_by_year, title_by_year_range, etc.)
2. Implement the `search_pa_list` function to handle pattern matching and responses  
3. Add at least one new movie to the database with proper formatting
4. Create a new pattern/action pair and add it to the pa_list
5. Ensure all provided assert statements pass
6. Complete the reflection questions below
7. Push your code to github for grading

## Reflection Questions

1. What are some key programming concepts or techniques that you learned while completing this assignment?
I learned how to use the debugger. Essentially, it allows you to run your code really really slowly so you can see what happens to all the variables as they do stuff. It is still kind of confusing to me but I get how it basically works.


2. How does the overall movie chatbot system work? Explain the flow from when a user types a query to when they receive an answer.
Step 1: a user types a query.
Step 2: the chatbot checks a short list of possible ways or templates that an answer may be formatted in, and checks them against the user's answer one by one.
Step 3: if the user's answer does not match any of the templates, the chatbot says "I don't understand". go back to step 1.
Step 4: if the user says "bye", chatbot says "So long!" and stops.
Step 5: if the user's answer does match, convert their query into a function and one or multiple parameters.
Step 6: run the function with said parameters.
Step 7: print the answer. Return to step 2.

3. What are some real-world applications where this type of pattern-matching chatbot system could be useful? How might you extend or improve this system for practical use?

I would implement a system that finds and ignores small typos. I would add more options for things you could say to it, and maybe a thing you can say to list out all the options for things it can say. This system could be useful for customer service, at least for the problems that are too simple to delegate to a neural net or even a human.