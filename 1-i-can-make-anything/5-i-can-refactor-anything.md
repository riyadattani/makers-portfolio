# I can refactor anything

##### Reflect: What does it mean to be able to refactor anything?

- Refactoring is to improve the quality of the code from something complex to something simpler, cleaner and conventional without changing the functionality or user experience of the code
- Follow TDD so that you have rigorous tests as a safety net to ensure you can refactor without changing the behaviour of the code

How to achieve this:

- Clean code that follows the Single Responsibility Principle (SRP):
  - When a class or method is doing more than one thing, it is not following SRP and should be broken up
  - Understand the responsibility of the model, views and controller. Try keep skinny controllers and remove unnecessary logic from the views
- Changeable code via encapsulation:
  - Encapsulation is when classes or objects hide information from other classes through private methods/ setters/ getters and therefore only expose the minimum amount of information necessary
  - Reduces the amount of testing required
- Readable code:
  - Anyone should be able to follow the code as each class/method/variable/etc is names accurately
  - Follow conventions depending on the language e.g. camelcase in Javascript, capital letters for classes etc
  - Code should be understandable without commenting
- DRY code - Don’t Repeat Yourself:
  - If you find yourself repeating some code then it can be extracted into its own method
- Make small changes at a time

##### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

- An example of code that follows SRP
- Example of code that is changeable via encapsulation
- An example of code that shows DRY code

**Q: Can you refactor anything? YES**

##### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

- Gilded Rose Kata from [this](https://github.com/emilybache/GildedRose-Refactoring-Kata/blob/master/ruby/gilded_rose.rb) to [this](https://github.com/riyadattani/GildedRose-Refactoring-Kata/blob/master/lib/gilded_rose.rb)
  - I used private methods to keep the code DRY and readable.
  - Before I started refactoring, I wrote behavioural tests based on the requirements as a safety net to ensure that the code I am refactoring does not change the functionality of the code.
- [Scrabble video](https://drive.google.com/open?id=1sI_RLcyqQDpBNkH_J8nX2fyg_4BNScDv)
  - Time 21:50: After debugging and my tests passing, I refactored my code using private methods i ruby so that the methods are readable.
- [Airport  challenge](https://github.com/riyadattani/airport_challenge/tree/master/lib)
  - The structure of the classes and methods are clean and follow SRP
  - To encapsulate the airport class and expose only the minimum amount of information needed, I used private methods where the class can read the capacity and the weather (the plane class or the weather class cannot access this information). Only the hangar variable is exposed.

##### What feedback have you had?

_Steven during process workshop_, “I like your use of private methods to refactor and make the code readable”
