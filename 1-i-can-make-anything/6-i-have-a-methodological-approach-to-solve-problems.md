# I have a methodical approach to solving problems

##### Reflect: What does it mean to have a methodical approach to solving problems?

- Firstly, break down the problem into smaller bite size issues
 - Understand the problem on a high level - you know you have understood it when you can explain the problem to someone else
- Diagram out the domain to view what is happening
- Research using google, read the docs, other reliable sources or even talk to pair to bounce ideas on what you will need to make the program work
- Look into a few approaches to tackle the problem and choose the best option to fulfill the criteria
- TDD each small goal of your chosen option
- Take a step back from time to time to view the program on an overarching level to check that you are achieving the overall goal


##### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

- Two large project showing the process of breaking down a problem into smaller bits,

**Q: Do you have a methodical approach to solving problems? YES**

##### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos).

- [Makersbnb](https://github.com/riyadattani/makersbnb/blob/master/lib/request.rb)
  - At first, modelling how the bookings and requests of spaces listed on a page was difficult. We broke down the requirements into smaller bits and looked at two perspectives:
    - The path if you were a landlord where you listed a space, you confirm or decline requests
    - The path if you were a user and you request a space and have a booking on a certain date
  - This was broken down further in terms of the model, view and controller
  - We faced a problem when trying to collate information from the database that lists the user, the owner, the space, the date and if this is confirmed. Instead of adding another table which essentially just draws information from other tables, we changed our approach and researched for the SQL command “JOIN” that creates a virtual table of the information we required
  - This saved us writing unnecessary code and made our code more efficient

- [Chitter challenge](https://github.com/riyadattani/chitter-challenge)
  - Modelled how app would be structured
  - Broke down the problem to features that relate to the user stories
  - These were broken down further - each created a unit test that was passed and eventually passing the feature
  - Challenge: to configure the PG gem which connects to the database
  - Refactored along the way to keep the code clean and easy to change.

##### What feedback have you had?

_Kim on MakersBnb_ when solving the problem explained above: “You are a focused individual and once you got into solving a problem, you had the grit and determination to continue. I really admire that. At first, you were using the walkthroughs, but once you got out of this zone, your mindset was more experimental which helped you to solve problems creatively. ”
