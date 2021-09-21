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

ಮುಖ್ಯ ರಿಯಾಕ್ಟ್ ಪರಿಕಲ್ಪನೆಗಳ ಕುರಿತು ಒಂದು ಹಂತ ಹಂತದ ಮಾರ್ಗದರ್ಶಿಯಲ್ಲಿ ಇದು ಮೊದಲ ಅಧ್ಯಾಯವಾಗಿದೆ. ನೇವಿಗೇಶನ್ ಸೈಡ್ಬಾರ್ನಲ್ಲಿ ನೀವು ಅದರ ಎಲ್ಲಾ ಅಧ್ಯಾಯಗಳ ಪಟ್ಟಿಯನ್ನು ಕಾಣಬಹುದು. ನೀವು ಮೊಬೈಲ್ ಸಾಧನದಿಂದ ಇದನ್ನು ಓದುತ್ತಿದ್ದರೆ, ನಿಮ್ಮ ಪರದೆಯ ಕೆಳಗಿನ ಬಲ ಮೂಲೆಯಲ್ಲಿರುವ ಗುಂಡಿಯನ್ನು ಒತ್ತುವುದರ ಮೂಲಕ ಸಂಚರಣೆ ಪ್ರವೇಶಿಸಬಹುದು.

ಈ ಅಧ್ಯಾಯದಲ್ಲಿ ಪ್ರತಿ ಅಧ್ಯಾಯವು ಹಿಂದಿನ ಅಧ್ಯಾಯಗಳಲ್ಲಿ ಪರಿಚಯಿಸಲ್ಪಟ್ಟ ಜ್ಞಾನವನ್ನು ನಿರ್ಮಿಸುತ್ತದೆ. **ಸೈಡ್ಬಾರ್ನಲ್ಲಿ ಕಂಡುಬರುವ ಕ್ರಮದಲ್ಲಿ "ಮುಖ್ಯ ಪರಿಕಲ್ಪನೆಗಳು" ಮಾರ್ಗದರ್ಶಿ ಅಧ್ಯಾಯಗಳನ್ನು ಓದುವ ಮೂಲಕ ನೀವು ಹೆಚ್ಚಿನ ಪ್ರತಿಕ್ರಿಯೆಯನ್ನು ಕಲಿಯಬಹುದು.** ಉದಾಹರಣೆಗೆ, ["ಪರಿಚಯಿಸುತ್ತಿದ್ದ JSX"](/docs/introducing-jsx.html) ಇದು ನಂತರದ ಮುಂದಿನ ಅಧ್ಯಾಯವಾಗಿದೆ.

<<<<<<< HEAD
## ಜ್ಞಾನ ಮಟ್ಟ ಊಹೆಗಳನ್ನು {#knowledge-level-assumptions}
=======
React is a JavaScript library, and so we'll assume you have a basic understanding of the JavaScript language. **If you don't feel very confident, we recommend [going through a JavaScript tutorial](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) to check your knowledge level** and enable you to follow along this guide without getting lost. It might take you between 30 minutes and an hour, but as a result you won't have to feel like you're learning both React and JavaScript at the same time.

>Note
>
>This guide occasionally uses some newer JavaScript syntax in the examples. If you haven't worked with JavaScript in the last few years, [these three points](https://gist.github.com/gaearon/683e676101005de0add59e8bb345340c) should get you most of the way.
>>>>>>> 0bb0303fb704147452a568472e968993f0729c28

ರಿಯಾಕ್ಟ್ ಒಂದು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಲೈಬ್ರರಿ, ಆದ್ದರಿಂದ ನೀವು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಭಾಷೆಯ ಮೂಲಭೂತ ತಿಳುವಳಿಕೆಯನ್ನು ಹೊಂದಿದ್ದೇವೆ ಎಂದು ನಾವು ಭಾವಿಸುತ್ತೇವೆ. **ನಿಮಗೆ ತುಂಬಾ ವಿಶ್ವಾಸವಿರದಿದ್ದರೆ, ನಿಮ್ಮ ಜ್ಞಾನ ಮಟ್ಟವನ್ನು ಪರಿಶೀಲಿಸಲು [ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಟ್ಯುಟೋರಿಯಲ್](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) ಮೂಲಕ ಹೋಗುವುದನ್ನು ನಾವು ಶಿಫಾರಸು ಮಾಡುತ್ತೇವೆ** ಮತ್ತು ಕಳೆದುಹೋಗದೆ ಈ ಮಾರ್ಗದರ್ಶಿಯನ್ನು ಅನುಸರಿಸಲು ನಿಮಗೆ ಅನುವು ಮಾಡಿಕೊಡುತ್ತದೆ. ಇದು ನಿಮ್ಮನ್ನು 30 ನಿಮಿಷಗಳು ಮತ್ತು ಒಂದು ಗಂಟೆಯೊಳಗೆ ತೆಗೆದುಕೊಳ್ಳಬಹುದು, ಆದರೆ ಪರಿಣಾಮವಾಗಿ ನೀವು ಒಂದೇ ಸಮಯದಲ್ಲಿ ರಿಯಾಕ್ಟ್ ಮತ್ತು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ಗಳನ್ನು ಕಲಿತಿರುವುದರಿಂದ ನೀವು ಅನುಭವಿಸಬೇಕಾಗಿಲ್ಲ.

>ಸೂಚನೆ
>
>ಈ ಮಾರ್ಗದರ್ಶಿ ಕೆಲವೊಮ್ಮೆ ಹೊಸ ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ ಸಿಂಟ್ಯಾಕ್ಸನ್ನು ಉದಾಹರಣೆಗಳಲ್ಲಿ ಬಳಸುತ್ತದೆ. ಕಳೆದ ಕೆಲವು ವರ್ಷಗಳಲ್ಲಿ ನೀವು ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್ನೊಂದಿಗೆ ಕೆಲಸ ಮಾಡದಿದ್ದರೆ, [ಈ ಮೂರು ಅಂಕಗಳು](https://gist.github.com/gaearon/683e676101005de0add59e8bb345340c) ನಿಮಗೆ ಹೆಚ್ಚು ದಾರಿ ಬೇಕು.

## ನಾವೀಗ ಆರಂಭಿಸೋಣ! {#lets-get-started}

ಸ್ಕ್ರಾಲ್ ಡೌನ್ ಮಾಡಿ, ಮತ್ತು ವೆಬ್ಸೈಟ್ ಅಡಿಟಿಪ್ಪಣಿಗೆ ಮುನ್ನ [ಈ ಮಾರ್ಗದರ್ಶಿ ಮುಂದಿನ ಅಧ್ಯಾಯಕ್ಕೆ](/docs/introducing-jsx.html) ನೀವು ಲಿಂಕ್ ಅನ್ನು ಕಾಣುತ್ತೀರಿ.

