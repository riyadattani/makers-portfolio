# I write code that is easy to change

##### Reflect: What does it mean to write code that is easy to change?

- Appropriate Naming!
- Model well and understand the responsibility of each class and the behaviour of each method
- Use names that correctly explain what it does
- DRY Code - this is achieved when you only need to change one thing when a change is needed
- SRP:
  - Classes should not be heavily coupled or a single class should not do everything. Think horizontally not vertically
  - A class should only do one thing so that when there are any changes made, the knock-on effect is minimised
- Encapsulation:
  - only the minimal amount of code should be exposed to other classes so that you can change the code internally without affecting the other classes
- Methods should be small (no longer than 5 lines)
- Use linters to keep code tidy and consistent


##### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

- Give two examples of code that you refactored so that it is easy to change

**Q: Do you write code that is easy to change? YES **

##### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

- [RPS challenge](https://github.com/riyadattani/rps-challenge)
  - Classes, methods and variables are clearly named
  - SRP achieved but could be better by extracting the winning beatmap into its own class
  - Methods are small and readable
- [Gilded Rose Kata](https://github.com/riyadattani/GildedRose-Refactoring-Kata/blob/master/lib/gilded_rose.rb)
  - DRY code as now the private methods can be easily changed since they are delegated out of the ‘update_quality’ method
  - Methods are small and tidy
  - Linter passes with no warnings
  - Named the private methods appropriately so that the ‘update_quality’ method is easy to read

##### What feedback have you had?

_Tome when reviewing RPS challenge,_ ‘You have well named routes, classes and methods. The code and tests are easy to read and I think I could edit them if needed to. You clearly have a good handle on MVC and single responsibility principle.’
