---
id: hello-world
title: Hello World
permalink: docs/hello-world.html
prev: cdn-links.html
next: introducing-jsx.html
---

ಚಿಕ್ಕದಾದ ರಿಯಾಕ್ಟ್ ಉದಾಹರಣೆಗೆ ಇದು ಕಾಣುತ್ತದೆ:

```js
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```

ಇದು ಪೇಜಿನಲ್ಲಿ  "Hello, world!" ಎಂದು ಹೆಡಿಂಗ್ ತೋರಿಸುತದೆ

[](codepen://hello-world)


ಆನ್ಲೈನ್ ಏಡಿಟೋರನ್ನು ತೆರೆಯಲು ಮೇಲಿನ ಲಿಂಕ್ ಅನ್ನು ಕ್ಲಿಕ್ ಮಾಡಿ. ಕೆಲವು ಬದಲಾವಣೆಗಳನ್ನು ಮಾಡಲು ಮುಕ್ತವಾಗಿರಿ, ಮತ್ತು ಅವರು ಔಟ್ಪುಟ್ ಅನ್ನು ಹೇಗೆ ಪ್ರಭಾವಿಸುತ್ತಾರೆ ಎಂಬುದನ್ನು ನೋಡಿ. ಈ ಗೈಡಿನಲ್ಲಿ ಹೆಚ್ಚಿನ ಪುಟಗಳು ಈ ರೀತಿಯ ಸಂಪಾದಿಸಬಹುದಾದ ಉದಾಹರಣೆಗಳನ್ನು ಹೊಂದಿರುತ್ತವೆ.

## ಈ ಗೈಡ್ ಅನ್ನು ಹೇಗೆ ಓದುವುದು {#how-to-read-this-guide}

ಈ ಮಾರ್ಗದರ್ಶಿಯಲ್ಲಿ, ನಾವು ರಿಯಾಕ್ಟ್ ಅಪ್ಲಿಕೇಶನ್ಗಳ ಬಿಲ್ಡಿಂಗ್ ಬ್ಲಾಕ್ಸ್ ಪರಿಶೀಲಿಸುತ್ತೇವೆ: ಎಲೆಮೆಂಟ್ಗಳು ಮತ್ತು ಕಾಂಪೊನೆಂಟ್ಗಳು. ಒಮ್ಮೆ ನೀವು ಅವುಗಳನ್ನು ಕರಗಿಸಿದರೆ, ಸಣ್ಣ ಪುನರ್ಬಳಕೆಯ ತುಣುಕುಗಳಿಂದ ಸಂಕೀರ್ಣ ಅಪ್ಲಿಕೇಶನ್ಗಳನ್ನು ನೀವು ರಚಿಸಬಹುದು.

>ಸಲಹೆ
>

ಈ ಮಾರ್ಗದರ್ಶಿ ** ಕಲಿಕೆಯ ಪರಿಕಲ್ಪನೆಗಳು ಹಂತ ಹಂತವಾಗಿ ** ಆದ್ಯತೆ ನೀಡುವ ಜನರಿಗೆ ವಿನ್ಯಾಸಗೊಳಿಸಲಾಗಿದೆ..
ಮಾಡುವ ಮೂಲಕ ನೀವು ತಿಳಿಯಲು ಬಯಸಿದಲ್ಲಿ, ನಮ್ಮ [ಪ್ರಾಯೋಗಿಕ ಟ್ಯುಟೋರಿಯಲ್](/tutorial/tutorial.html). ಈ ಮಾರ್ಗದರ್ಶಿ ಮತ್ತು ಟ್ಯುಟೋರಿಯಲ್ ಪರಸ್ಪರ ಪೂರಕವಾಗಬಹುದು.

This is the first chapter in a step-by-step guide about main React concepts. You can find a list of all its chapters in the navigation sidebar. If you're reading this from a mobile device, you can access the navigation by pressing the button in the bottom right corner of your screen.

Every chapter in this guide builds on the knowledge introduced in earlier chapters. **You can learn most of React by reading the “Main Concepts” guide chapters in the order they appear in the sidebar.** For example, [“Introducing JSX”](/docs/introducing-jsx.html) is the next chapter after this one.

## Knowledge Level Assumptions {#knowledge-level-assumptions}

React is a JavaScript library, and so we'll assume you have a basic understanding of the JavaScript language. **If you don't feel very confident, we recommend [going through a JavaScript tutorial](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) to check your knowledge level** and enable you to follow along this guide without getting lost. It might take you between 30 minutes and an hour, but as a result you won't have to feel like you're learning both React and JavaScript at the same time.

>Note
>
>This guide occasionally uses some of the newer JavaScript syntax in the examples. If you haven't worked with JavaScript in the last few years, [these three points](https://gist.github.com/gaearon/683e676101005de0add59e8bb345340c) should get you most of the way.


## Let's Get Started! {#lets-get-started}

Keep scrolling down, and you'll find the link to the [next chapter of this guide](/docs/introducing-jsx.html) right before the website footer.


