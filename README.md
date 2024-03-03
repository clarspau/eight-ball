# Magic Eight Ball Simulation

In this exercise, you'll create a simulation of the classic kid's toy, the [Magic Eight Ball](https://en.wikipedia.org/wiki/Magic_8-Ball).

## Overview

This application will consist of two components:

- **App**: A simple component that just renders an *EightBall* component.
- **EightBall**: The component for the magic eight ball.

## Step One: *EightBall* Component

The *EightBall* component will simulate the behavior of a Magic Eight Ball. It will display a black ball with the initial message "Think of a Question". When clicked, it should choose a random answer and change its color accordingly.

### Usage

The *EightBall* component should take a single property, `answers`, which should be an array of objects containing the possible answers and their corresponding colors.

```jsx
const answers = [
  { msg: "It is certain.", color: "green" },
  { msg: "It is decidedly so.", color: "green" },
  { msg: "Without a doubt.", color: "green" },
  { msg: "Yes - definitely.", color: "green" },
  { msg: "You may rely on it.", color: "green" },
  { msg: "As I see it, yes.", color: "green" },
  { msg: "Most likely.", color: "green" },
  { msg: "Outlook good.", color: "green" },
  { msg: "Yes.", color: "green" },
  { msg: "Signs point to yes.", color: "goldenrod" },
  { msg: "Reply hazy, try again.", color: "goldenrod" },
  { msg: "Ask again later.", color: "goldenrod" },
  { msg: "Better not tell you now.", color: "goldenrod" },
  { msg: "Cannot predict now.", color: "goldenrod" },
  { msg: "Concentrate and ask again.", color: "goldenrod" },
  { msg: "Don't count on it.", color: "red" },
  { msg: "My reply is no.", color: "red" },
  { msg: "My sources say no.", color: "red" },
  { msg: "Outlook not so good.", color: "red" },
  { msg: "Very doubtful.", color: "red" },
];
```

### Functionality

- The *EightBall* component will initially display a black ball with the message "Think of a Question".
- When clicked, it will randomly select one of the predefined answers and change its color accordingly.
- The color and message text should update dynamically upon each click.

### Implementation Details

- The *EightBall* component will maintain state to keep track of the current color and message text, which will initially be "black" and "Think of a Question", respectively.
- Upon clicking, the component will select a random message from the provided answers array and update its state accordingly.
- The component will update its appearance based on the selected message's color.

Let's get started building our Magic Eight Ball simulation! 🎱✨
