---
id: pure-render-mixin
title: PureRenderMixin
permalink: docs/pure-render-mixin.html
layout: docs
category: Add-Ons
---

> Note:
>
> `PureRenderMixin` is a legacy add-on. Use [`React.PureComponent`](/docs/react-api.html#reactpurecomponent) instead.

**ಆಮದು ಮಾಡಲಾಗುತ್ತಿದೆ**

```javascript
import PureRenderMixin from 'react-addons-pure-render-mixin'; // ES6
var PureRenderMixin = require('react-addons-pure-render-mixin'); // ES5 with npm
```

## ಅವಲೋಕನ {#ಅವಲೋಕನ} 

ನಿಮ್ಮ ರಿಯಾಕ್ಟ್ ಕಾಂಪೊನೆಂಟ್‌ನ ರೆಂಡರ್ ಕಾರ್ಯವು ಅದೇ ರಂಗಪರಿಕರಗಳು ಮತ್ತು ಸ್ಥಿತಿಯನ್ನು ನೀಡಿದ ಅದೇ ಫಲಿತಾಂಶವನ್ನು ನೀಡಿದರೆ, ಕೆಲವು ಸಂದರ್ಭಗಳಲ್ಲಿ ಕಾರ್ಯಕ್ಷಮತೆ ವರ್ಧನೆಗೆ ನೀವು ಈ ಮಿಕ್ಸಿನ್ ಅನ್ನು ಬಳಸಬಹುದು.

ಉದಾಹರಣೆ:

```js
const createReactClass = require('create-react-class');

createReactClass({
  mixins: [PureRenderMixin],

  render: function() {
    return <div className={this.props.className}>foo</div>;
  }
});
```

Under the hood, the mixin implements [shouldComponentUpdate](/docs/component-specs.html#updating-shouldcomponentupdate), in which it compares the current props and state with the next ones and returns `false` if the equalities pass.

> ಸೂಚನೆ:
>
> ಇದು ಕೇವಲ ಆಳವಿಲ್ಲದ ವಸ್ತುಗಳನ್ನು ಹೋಲಿಸುತ್ತದೆ. ಇವು ಸಂಕೀರ್ಣ ದತ್ತಾಂಶ ರಚನೆಗಳನ್ನು ಹೊಂದಿದ್ದರೆ, ಇದು ಆಳವಾದ ವ್ಯತ್ಯಾಸಗಳಿಗೆ ತಪ್ಪು-ನಿರಾಕರಣೆಗಳನ್ನು ಉಂಟುಮಾಡಬಹುದು. ಸರಳವಾದ ರಂಗಪರಿಕರಗಳು ಮತ್ತು ಸ್ಥಿತಿಯನ್ನು ಹೊಂದಿರುವ ಘಟಕಗಳಲ್ಲಿ ಮಾತ್ರ ಬೆರೆಸಿ, ಅಥವಾ ಆಳವಾದ ದತ್ತಾಂಶ ರಚನೆಗಳು ಬದಲಾಗಿವೆ ಎಂದು ನಿಮಗೆ ತಿಳಿದಾಗ `ಫೋರ್ಸ್‌ಅಪ್ಡೇಟ್ ()` ಅನ್ನು ಬಳಸಿ. ಅಥವಾ, ನೆಸ್ಟೆಡ್ ಡೇಟಾದ ವೇಗದ ಹೋಲಿಕೆಗೆ ಅನುಕೂಲವಾಗುವಂತೆ [ಬದಲಾಗದ ವಸ್ತುಗಳು] (https://facebook.github.io/immutable-js/) ಬಳಸುವುದನ್ನು ಪರಿಗಣಿಸಿ.
>
> ಇದಲ್ಲದೆ, `ಕಾಂಪೊನೆಂಟ್ ಅಪ್‌ಡೇಟ್` ಇಡೀ ಘಟಕ ಸಬ್‌ಟ್ರೀಗಾಗಿ ನವೀಕರಣಗಳನ್ನು ಬಿಟ್ಟುಬಿಡುತ್ತದೆ. ಎಲ್ಲಾ ಮಕ್ಕಳ ಘಟಕಗಳು ಸಹ "ಶುದ್ಧ" ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ.
