# ES6 CLASSES: Gladiator Arena ⚔ 🛡

![are you not entertained](./assets/entertained.gif)

The Emperor has commissioned you to build a Gladiator Arena!! You'll be using your newfound ability to create ES6 classes to help them out. The Emperor has also provided some handy tests for you, written in Mocha and Chai, to help you know when you'll be done...

## 🚀 Before you start...

- Within the `gladiator` directory, run `npm install` to install our lovely testing dependencies
- Within the `gladiator` directory, run `npm test` to run the test suite. Yikes!! Lots of red.
- You'll be working in both `gladiator.js` and `arena.js`. 
- Remember to export your `Gladiator` and `Arena` classes using `module.exports` so they can be properly tested!!!
- If you can't figure out one of the steps, try writing some pseudocode in a comment in your file. You never know, it may come to you...
- You can also take a look at the tests to see if you get any hints that way...
- Also, feel free to comment out sections of the tests while you're working on other parts of the assignment. There are some bonuses that have been commented out already.

### 🚀 Completion looks like...

- All your tests are green!

### 🚀 Your submission should include...

- A pull request to this repository.
- Questions, comments, concerns... you know the drill.

## This homework is due 🚨🚨 TONIGHT at 11PM!! 🚨🚨

# ⚔ INSTRUCTIONS ⚔

Hint!! These should give you a pretty good overview of what you need to do, but the tests are more descriptive.

## Part 1 - The Gladiator

In `gladiator.js`, create a `Gladiator` class that has the following properties:

- a `name`
- a `weapon` (one of Spear, Club, Trident)

The properties should be passed into the class when it is created.

> Ideally the Gladiator class shouldn't accept anything as a weapon except the strings `Spear`, `Club`, and `Trident`... head on down to [the bonus](#bonus-) if you want to tackle that now.

## Part 2 - The Arena

In `arena.js`, create an `Arena` class that meets the following conditions:

1. An arena has a name. This is passed in when the class is created.
2. The name should be capitalized.
3. An arena can have gladiators. This is initialized as an empty array.
4. You can add a gladiator to the arena.
5. The arena should never have more than 2 gladiators in it at a time.
6. If there are two gladiators in the arena, you can call a `fight` method that results in the elimination of one of the gladiators from the arena.
  - Winning conditions:
    - Trident beats Spear
    - Spear beats Club
    - Club beats Trident
    - If the two gladiators have the same weapon, they are both eliminated.
  - (If you're having a rough time thinking through this, just think about Rock Paper Scissors...)


##  Bonus!!!!! 💪💪

Uncomment the bonus sections of the tests when you start working on these!!

- Add a method to remove gladiators from the arena by name
- Update your winning conditions so that if the gladiator named "Maximus" is in the fight, he wins.
- Add a method to check to see if the crowd is entertained (`.entertained()`). The crowd is only entertained if Maximus is in the arena.

## ✨ Double Bonus!!!!!!!! ✨

How could you prevent creating Gladiators with a different weapon? e.g. `new Gladiator('J','Taco')` throws an error. (Maybe [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error) has something to say about this...)

What other types of errors can you think of?? Here's a few:
- What if you try to add something to an arena's gladiators that's not an object created with the `Gladiator` class?
- What if you try to run the `fight` method without two gladiators in the arena?