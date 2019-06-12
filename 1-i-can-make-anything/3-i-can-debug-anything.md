# I can debug anything

##### Reflect: What does it mean to be able to debug anything?

A step-by-step process that can be applied to any debugging situation.

My debugging process:
- Identify the useful information within the error message and understand it
    - If you don't understand it, look it up
- Follow the stack trace to find where the source of the bug is in the code
- Tighten the loop and get visibility by revealing what the code is doing using ‘p’ in Ruby or ‘console.log’ in Javascript, save_and_open in Capybara etc
- Identify what is unexpected
- Go back through the code and identify two points between which the problem is occuring - inspect this section further by getting more visibility
- Tighten the loop again - follow from step 3 - until you have identified the issue
  - Sometimes it may be difficult to tighten the loop and I would comment out large bits of the code to isolate the part of the code where the problem is occuring
  - Other times, there is something obvious that is overlooked and so I would timebox the amount of time I spend debugging and take a break. E.g. after 20-30 minutes of following the process, I would step away from my computer
- Fix the bug


##### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

- A video following each step of my debugging process.
- An example of debugging in something unfamiliar.

**Q: Can you debug anything? YES**

##### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

- [Scrabble video](https://drive.google.com/open?id=1sI_RLcyqQDpBNkH_J8nX2fyg_4BNScDv)
  - Video time: 18:15 - when I got a failing test which I did not know the cause of, I show my debugging process by tightening the loop to gain visibility and eventually solving the problem
- Debugging workshop examples [attach folder]
  - This was something unfamiliar to me
  - During Alice’s debugging workshop, I debugged the code using the console:
    - I tracked the bug by inputting ‘debugger’ at the top of the code
    - The console revealed the area at which the code is breaking
    - Capybara also had a stack trace of the source of the bug
    - I gained visibility by using ‘p’ in ruby and tightened the loop
    - I identified the problem and fixed it

##### What feedback have you had?

[Acebook](https://github.com/riyadattani/acebook-winklebossnit/blob/master/spec/controllers/posts_controller_spec.rb)

Since we used the devise gem to generate our users, login and logout page, existing controller tests failed when this was generated. To debug these failing tests, I used FactoryBot to create a new user.

_Tome’s feedback on debugging this:_  “Riya was pivotal to the success of the team, bringing light-hearted pragmatism to the team that set a great example and guided the way we worked together towards agility. She exemplified this when we encountered a blocker that the whole team had mobbed around and was struggling to get past. ”
