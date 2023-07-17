

### Defining helper functions

```javascript
const setStartGameInvalidState = () => {
...
}

const userExists = (username) => {
...
}

const checkAnswer = (question, userAnswer, correct) => {
...
}

const loadQuestionAndAnswers = () => {
...
}
```

These are helper functions defined to manage the game state, validate user input, update game statistics, and load questions and answers. They are used in various parts of the code to perform these tasks.

### Adding event listeners

```javascript
nextSectionTriggers.forEach((trigger) => {
  trigger.addEventListener('click', (e) => nextSectionClickListener(e))
})

answers.forEach((answer) => {
  answer.addEventListener('click', (e) => toggleSelectIndicator(e))
})

usernameInput.addEventListener('input', checkUsernameValidity)
usernameInput.addEventListener('blur', checkUsernameValidity)

playAgainBtn.addEventListener('click', () => window.location.reload())
```

These lines add event listeners to various DOM elements. When the user interacts with these elements (for example, by clicking a button or entering input), the corresponding event listener function is triggered. For instance, when the "Play Again" button is clicked, the page is reloaded.
